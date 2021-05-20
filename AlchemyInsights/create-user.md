---
title: Kurti vartotoją
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569739"
---
# <a name="create-user"></a>Kurti vartotoją

**PRANEŠIMAS:**

- ["WebView" prisijungimo palaikymo nutraukimas iš "Google" nuo 2021 m. sausio 4 d.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Patikrinkite, ar jūsų programoms gali turėti įtakos ["Google" suderinamumo](https://go.microsoft.com/fwlink/?linkid=2157323) tikrinimo rekomendacijos.
- Įsitikinkite, kad naudojate sistemos žiniatinklio rodinį arba sistemos naršyklę prisijungę prie vartotojų naudodami vartotojų "Google" paskyras. Daugiau informacijos žr. [Prisijungimo prie programos (-ų) naudojant tik "Chrome" naršyklę problemos.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Negaliu sukurti naujo vartotojo savo "Azure AD" kataloge**

1. Įsitikinkite, kad turite teisę sukurti naują standartinį vartotoją. Tik visuotinis administratorius arba vartotojo administratoriaus vaidmuo "Azure Active Directory" (AD) gali sukurti naują standartinį vartotoją. Jei neturite vieno iš šių vaidmenų, paprašykite administratoriaus įtraukti jus į vieną iš šių vaidmenų arba sukurti naują vartotojo paskyrą už jus.
1. Įsitikinkite, kad vartotojo vardas yra domene, kuris patvirtintas jūsų "Azure AD". Jei "Azure AD" neturite patikrintų pasirinktinių domenų vardų, galite naudoti "Azure AD" pradinį domeną, kuris baigiasi *.onmicrosoft.com.
1. Įsitikinkite, kad vartotojo vardas yra domene, kuris nėra susietas su "Azure AD" iš jūsų vietinio AD. Vartotojų negalima įtraukti į debesį su domenų vardais, kurie yra išoriniai iš vietinės.
1. Įsitikinkite, kad joks kitas vartotojas ar kontaktas dar neturi vartotojo vardo, kurį norite priskirti naujam vartotojui. Vartotojų vardai turi būti unikalūs visoje "Azure AD".
1. Žr. ["Azure AD" vaidmenys ir "Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD" administratoriai.
1. Peržiūrėkite ["Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD" domenų vardus.
1. Peržiūrėkite [audito žurnalus,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) kad pamatytumėte išsamesnę informaciją apie neseniai sukurtą arba panaikintus vartotoją, pvz., kas atliko veiksmą ir kada.
1. Daugiau informacijos apie naujų vartotojų įtraukimą žr. ["Azure" portalo naudojimas kuriant naują vartotoją "Azure AD".](/azure/active-directory/active-directory-users-create-azure-portal)
1. ["Azure AD" administravimo vaidmenys:](/azure/active-directory/active-directory-assign-admin-roles)administratoriaus vaidmens teisės "Azure Active Directory"
1. Taip pat galite [naudoti "Azure AD PowerShell", kad sukurtumėte naują vartotoją.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
