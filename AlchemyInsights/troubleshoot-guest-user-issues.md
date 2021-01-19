---
title: Svečio vartotojų problemų šalinimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901596"
---
# <a name="troubleshoot-guest-user-issues"></a>Svečio vartotojų problemų šalinimas

1. Patarimų, kaip valdyti svečio prieigą prie taikomųjų programų, ieškokite [svečio prieigos valdymas naudojant "AZURE ad Access" atsiliepimus](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Įtraukite Svečių vartotojus į savo katalogą "Azure" portale](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): šiame "QuickStart" į "Azure AD" katalogą į "Azure AD" portalą įtrauksite naują svečio portalą naudodami "Azure" portalą, išsiųstumėte kvietimą ir pamatytumėte, kaip atrodo svečio vartotojo kvietimo išpirkimo procesas.
1. [Įtraukti svečio vartotoją su "PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)": šiame "QuickStart" naudokite komandą New-AzureADMSInvitation, kad įtrauktumėte vieną svečio vartotoją į savo "Azure" nuomotoją.
1. Norėdami sužinoti, kaip priskirti vartotojus ir grupes, įmonės taikomąsias programas "Azure Active Directory" ("Azure AD"), iš "Azure" portalo arba naudodami "PowerShell", žr. ["Azure Active Directory" taikomosios programos vartotojo priskyrimo valdymas](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. "Azure Active Directory" ("Azure AD") B2B bendradarbiavimas veikia su daugeliu programų, kurios integruojasi su "Azure AD". Šiame [straipsnyje](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)pateikiame instrukcijas, kaip konfigūruoti kai kurias populiarias "SaaS" taikomąsias programas, skirtas naudoti su "AZURE ad B2B".
1. Kaip organizacija, naudojanti "Azure Active Directory" ("Azure AD") B2B bendradarbiavimo galimybes, siekiant pakviesti Svečių vartotojus iš partnerių organizacijų į "Azure AD", dabar galite pateikti šiems B2B vartotojams prieigą prie vietinių taikomųjų programų. Šios vietinio naudojimo programos gali naudoti SAML pagrįstą autentifikavimą arba integruotą "Windows" autentifikavimą (IWA) su "Kerberos" ribojtu perdavimu (KCD). Daugiau informacijos ieškokite ["AZURE AD" prieigos prie vietinių taikomųjų programų B2B vartotojų suteikimas](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Sužinokite, kaip [suteikti vietinio valdymo partnerio paskyras prieigą prie debesies išteklių naudojant "AZURE ad B2B Collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)".