---
title: Vartotojo kūrimas
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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747020"
---
# <a name="create-user"></a>Vartotojo kūrimas

**SKELBIMU**

- [Žiniatinklio rodinio prisijungimo palaikymo palaikymas iš "Google" nuo sausio 4 d., 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Patikrinkite, ar jūsų programėlėms gali turėti įtakos šios ["Google" rekomendacijos](https://go.microsoft.com/fwlink/?linkid=2157323) dėl suderinamumo bandymų.
- Įsitikinkite, kad prisijungę prie vartotojų "Google" paskyrų naudojate sistemos žiniatinklio rodinį arba sistemos naršyklę. Daugiau informacijos ieškokite straipsnyje [prisijungimo prie taikomosios programos (-ų) problemos naudojant tik "Chrome" naršyklę](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Negaliu sukurti naujo vartotojo "Azure AD" kataloge**

1. Įsitikinkite, kad turite teisę sukurti naują standartinį vartotoją. Tik visuotinis administratorius arba vartotojo administratorius vaidmuo "Azure Active Directory" (AD) gali sukurti naują standartinį vartotoją. Jei nesate nė vieno iš šių vaidmenų, paprašykite administratoriaus, kad įtrauktumėte jus į vieną iš šių vaidmenų arba sukurtumėte naują vartotojo paskyrą.
1. Įsitikinkite, kad vartotojo vardas yra domene, kuris patikrintas jūsų "Azure AD". Jei "Azure AD" neturite jokių patikrintų pasirinktinio domenų vardų, galite naudoti "Azure AD" pradinį domeną, kuris baigiasi *. onmicrosoft.com.
1. Įsitikinkite, kad vartotojo vardas priklauso domenui, kuris nėra sujungtas su "Azure AD" iš vietinio skelbimo. Vartotojų negalima įtraukti į debesį su domenų pavadinimais, kurie yra susieti vietinėje organizacijoje.
1. Įsitikinkite, kad joks kitas vartotojas arba kontaktas jau turi vartotojo vardą, kurį norite priskirti naujam vartotojui. Vartotojų vardai turi būti unikalūs "Azure AD".
1. Ieškokite "Azure AD" [vaidmenų ir administratorių](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) "Azure AD".
1. Peržiūrėkite "Azure AD" [domenų vardus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) .
1. Peržiūrėkite [audito žurnalus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , kad matytumėte išsamesnę informaciją apie neseniai sukurtą arba panaikintą vartotoją, pvz., kas atliko veiksmą ir kada.
1. Daugiau informacijos apie naujų vartotojų įtraukimą ieškokite " [Azure" portalo naudojimas kuriant naują vartotoją "AZURE ad](/azure/active-directory/active-directory-users-create-azure-portal)".
1. "Azure [AD" administravimo vaidmenys](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): "Azure Active Directory" administratoriaus vaidmens teisės
1. Taip pat galite [naudoti "AZURE ad PowerShell", kad sukurtumėte naują vartotoją](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
