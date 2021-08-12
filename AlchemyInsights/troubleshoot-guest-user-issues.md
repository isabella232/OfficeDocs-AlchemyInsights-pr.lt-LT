---
title: Svečių vartotojų trikčių šalinimas
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939387"
---
# <a name="troubleshoot-guest-user-issues"></a>Svečių vartotojų trikčių šalinimas

1. Patarimų, kaip valdyti svečio prieigą prie taikomųjų programų, žr. [Svečio prieigos valdymas naudojant "Azure AD" prieigos atsiliepimus](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Įtraukite svečių vartotojus į savo katalogą ["Azure" portale:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)Šiame greityje įtrauksite naują svečio vartotoją į savo "Azure AD" katalogą naudodami "Azure" portalą, siųsite kvietimą ir pamatysite, kaip atrodo svečio kvietimo išpirkimo procesas.
1. [Įtraukite svečio vartotoją naudodami "PowerShell":](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)šiame sparčiosios paleisties lange naudosite komandą New-AzureADMSInvitation vieną svečio vartotoją įtraukti į "Azure" nuomotoją.
1. Norėdami sužinoti, kaip priskirti vartotojus ir grupes įmonės programoms ""Azure Active Directory"" ("Azure AD"), iš "Azure" portalo arba naudojant "PowerShell", žr. ""Azure Active Directory"" taikomosios programos vartotojų [priskyrimo valdymas.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. "Azure Active Directory" ("Azure AD") B2B bendradarbiavimas veikia su daugeliu programų, integruojamų su "Azure AD". Šiame straipsnyje [pateikiame](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)instrukcijas, kaip konfigūruoti kai kurias populiarias "SaaS" programas, skirtas naudoti su "Azure AD B2B".
1. Kaip organizacija, kuri naudoja "Azure Active Directory" ("Azure AD") B2B bendradarbiavimo galimybes pakviesti svečių vartotojus iš partnerių organizacijų į "Azure AD", dabar galite suteikti šiems B2B vartotojams prieigą prie vietinių programų. Šios vietinės programos gali naudoti SAML pagrįstą autentifikavimą arba integruotą Windows autentifikavimą (IWA) su "Kerberos" apribotuoju perdavimu (KCD). Daugiau informacijos žr. [B2B vartotojų suteikimas "Azure AD" prieigai prie jūsų vietinės programos](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Sužinokite, [kaip suteikti lokaliai valdomų partnerių paskyroms prieigą prie debesies išteklių naudojant "Azure AD B2B" bendradarbiavimą.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)