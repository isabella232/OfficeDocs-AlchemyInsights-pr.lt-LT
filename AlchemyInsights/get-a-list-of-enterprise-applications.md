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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404927"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="5f9c2-102">Gaukite "Enterprise" taikomųjų programų sąrašą</span><span class="sxs-lookup"><span data-stu-id="5f9c2-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="5f9c2-103">Norėdami **gauti įmonės taikomųjų programų** sąrašą (visas taikomąsias programas arba filtruoti pagal rodomą pavadinimą, ID, identifikatorių URI ir kt.) naudodami "PowerShell" komandą, žr. [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="5f9c2-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="5f9c2-104">Norėdami gauti pagrindinių tarnybos objektų sąrašą (visus objektus arba filtruoti pagal ID) naudodami "PowerShell" komandą, žr. [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="5f9c2-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="5f9c2-105">Jei norite gauti **SAML sukonfigūruotų programų sąrašą, "PowerShell" scenarijai gali** jums padėti:</span><span class="sxs-lookup"><span data-stu-id="5f9c2-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="5f9c2-106">Kiekviena taikomoji programa būtų "OAuth" programa arba SAML programa (tiek galerijos, tiek ne galerijos programos) turėtų du objektus, sukurtus AAD, kai jų registracija įvyks.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="5f9c2-107">Vienas iš jų vadinamas programos objektu, o kitas – pagrindinis tarnybos objektas.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="5f9c2-108">Kai išmesite pagrindinio tarnybos objekto ypatybes naudodami "PowerShell", pastebėsite, kad kiekviena taikomoji programa turi tam tikrą skaičių žymių, susietų su juo, pvz.:</span><span class="sxs-lookup"><span data-stu-id="5f9c2-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="5f9c2-109">"OAuth" taikomosios programos turėtų žymę,**vadinamą "WindowsAzureActiveDirectoryIntegratedApp"**</span><span class="sxs-lookup"><span data-stu-id="5f9c2-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="5f9c2-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"**</span><span class="sxs-lookup"><span data-stu-id="5f9c2-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="5f9c2-111">Ne galerijos SAML programos turėtų žymę, vadinamą **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication"**</span><span class="sxs-lookup"><span data-stu-id="5f9c2-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="5f9c2-112">Taigi, galite naudoti šias žymes ir sužinoti, kokios programos ji yra.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="5f9c2-113">Žymė **"WindowsAzureActiveDirectoryIntegratedApp"** yra įprasta visų tipų programėlėms.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="5f9c2-114">Galite naudoti šį fragmentą norėdami išvardyti visas SAML programas (galeriją ir ne galeriją):</span><span class="sxs-lookup"><span data-stu-id="5f9c2-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="5f9c2-115">Daugiau informacijos žr. "Azure AD" taikomųjų programų, kuriose įgalinta [SAML, identifikavimas.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="5f9c2-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="5f9c2-116">**Raskite ir išvardikite tik** žiniatinklio taikomąsias programas: naudokite toliau pateiktą komandą, kad gautumėte visas "Azure AD" taikomąsias programas su programos tipu "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="5f9c2-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="5f9c2-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="5f9c2-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="5f9c2-118">**Raskite ir išvardikite tik vietinės** programos: vykdykite šią komandą, kad gautumėte visas vietinių klientų (kompiuterio / mobiliojo įrenginio) programas.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="5f9c2-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="5f9c2-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="5f9c2-120">**Eksportuoti visą registruotą "Azure AD"** taikomosios programos informaciją į CSV: toliau pateikta komanda eksportuoja visas "Azure AD" programas su reikiama informacija į csv failą:</span><span class="sxs-lookup"><span data-stu-id="5f9c2-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="5f9c2-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="5f9c2-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="5f9c2-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="5f9c2-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="5f9c2-123">**Reikia eksportuoti nenaudojamų "Azure" programų** sąrašą – audito ataskaita</span><span class="sxs-lookup"><span data-stu-id="5f9c2-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="5f9c2-124">"Azure AD" programų žurnalus gali rodyti tik iki 30 dienų, jei turite "Azure AD Premium" licenciją.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="5f9c2-125">Turite dvi parinktis, kaip išsaugoti duomenis ilgiau nei 30 dienų.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="5f9c2-126">Galite naudoti ["Azure AD" ataskaitų API](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) norėdami programiškai nuskaityti duomenis ir saugoti juos duomenų bazėje.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="5f9c2-127">Taip pat galite integruoti audito žurnalus į trečiosios šalies SIEM sistemą.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="5f9c2-128">Taip pat galite atsisiųsti visų programų ir priklausomų programų sąrašą dalyje "Azure Active directory>App Registrations">Atsisiųsti>Visos taikomosios programos / priklauso taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="5f9c2-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="5f9c2-129">Norėdami gauti taikomųjų programų sąrašą per MS Graph, žr. Taikomųjų programų sąrašas [– "Microsoft Graph v1.0"](https://docs.microsoft.com/graph/api/application-list) ir programos išteklių [tipas – "Microsoft Graph v1.0".](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="5f9c2-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
