---
title: Taikomųjų programų naikinimas arba atkūrimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102579"
---
# <a name="delete-or-restore-applications"></a>Taikomųjų programų naikinimas arba atkūrimas

**Norėdami panaikinti taikomąją programą iš "Azure AD" nuomotojo:**

1. "Azure **AD" portale** pasirinkite **Įmonės programos**. Tada raskite ir pasirinkite taikomąją programą, kurią norite panaikinti.
2. Kairiojoje **srityje** esančioje sekcijoje Tvarkyti pasirinkite **Ypatybės**.
3. Pasirinkite **Naikinti**, tada pasirinkite **Taip,** kad patvirtintumėte, kad norite panaikinti programą iš "Azure AD" nuomotojo.

Daugiau informacijos, kaip panaikinti taikomąją programą, [žr. "Quickstart": taikomosios programos naikinimas iš "Azure Active Directory" ("Azure AD") nuomotojo](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

"PowerShell" cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) pašalina programos tarpinio serverio konfigūracijas iš konkrečios ""Azure Active Directory"" taikomosios programos ir gali visiškai panaikinti taikomąją programą, jei nurodyta.

**Panaikinę taikomąją programą galite atkurti naudodami** "PowerShell". Kai bus nustatyta programa, kurią norite atkurti, galėsite ją atkurti naudodami ["Restore-AzureADDeletedApplication".](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
