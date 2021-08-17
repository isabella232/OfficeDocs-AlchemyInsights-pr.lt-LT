---
title: Gaukite "Enterprise" taikomųjų programų sąrašą
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116736"
---
# <a name="get-a-list-of-enterprise-applications"></a>Gaukite "Enterprise" taikomųjų programų sąrašą

1. Norėdami **gauti įmonės taikomųjų programų** sąrašą (visas taikomąsias programas arba filtruoti pagal rodomą pavadinimą, ID, identifikatorių URI ir kt.) naudodami "PowerShell" komandą, žr. [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Norėdami gauti pagrindinių tarnybos objektų sąrašą (visus objektus arba filtruoti pagal ID) naudodami "PowerShell" komandą, žr. [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Jei norite gauti **SAML sukonfigūruotų programų sąrašą, "PowerShell" scenarijai gali** jums padėti:

    Kiekviena taikomoji programa būtų "OAuth" programa arba SAML programa (tiek galerijos, tiek ne galerijos programos) turėtų du objektus, sukurtus AAD, kai jų registracija įvyks. Vienas iš jų vadinamas programos objektu, o kitas – pagrindinis tarnybos objektas. Kai išmesite pagrindinio tarnybos objekto ypatybes naudodami "PowerShell", pastebėsite, kad kiekviena taikomoji programa turi tam tikrą skaičių žymių, susietų su juo, pvz.:

    - "OAuth" taikomosios programos turėtų žymę,**vadinamą "WindowsAzureActiveDirectoryIntegratedApp"**
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**
    - Ne galerijos SAML programos turėtų žymę, vadinamą **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**

    Taigi, galite naudoti šias žymes ir sužinoti, kokios programos ji yra. Žymė **"WindowsAzureActiveDirectoryIntegratedApp"** yra įprasta visų tipų programėlėms. Galite naudoti šį fragmentą norėdami išvardyti visas SAML programas (galeriją ir ne galeriją):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Daugiau informacijos žr. "Azure AD" taikomųjų programų, kuriose įgalinta [SAML, identifikavimas.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Raskite ir išvardikite tik** žiniatinklio taikomąsias programas: naudokite toliau pateiktą komandą, kad gautumėte visas "Azure AD" taikomąsias programas su programos tipu "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Raskite ir išvardikite tik vietinės** programos: vykdykite šią komandą, kad gautumėte visas vietinių klientų (kompiuterio / mobiliojo įrenginio) programas.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Eksportuoti visą registruotą "Azure AD"** taikomosios programos informaciją į CSV: toliau pateikta komanda eksportuoja visas "Azure AD" programas su reikiama informacija į csv failą:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Reikia eksportuoti nenaudojamų "Azure" programų** sąrašą – audito ataskaita

    "Azure AD" programų žurnalus gali rodyti tik iki 30 dienų, jei turite "Azure AD" Premium licenciją.
    Turite dvi parinktis, kaip išsaugoti duomenis ilgiau nei 30 dienų. Galite naudoti ["Azure AD" ataskaitų API](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) norėdami programiškai nuskaityti duomenis ir saugoti juos duomenų bazėje. Taip pat galite integruoti audito žurnalus į trečiosios šalies SIEM sistemą.

    Taip pat galite atsisiųsti visų programų ir priklausomų programų sąrašą dalyje "Azure Active directory>App Registrations">Atsisiųsti>Visos taikomosios programos / priklauso taikomosios programos.

    Norėdami gauti taikomųjų programų sąrašą per MS "Graph", žr. Programų sąrašas [– "Microsoft "Graph" v1.0"](https://docs.microsoft.com/graph/api/application-list) ir programos išteklių [tipas – "Microsoft "Graph" v1.0".](https://docs.microsoft.com/graph/api/resources/application)
