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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014904"
---
# <a name="delete-or-restore-applications"></a>Taikomųjų programų naikinimas arba atkūrimas

**Norėdami panaikinti taikomąją programą iš "AZURE AD" nuomotojo**:

1. " **AZURE AD" portale** pasirinkite **įmonės taikomosios programos**. Tada Raskite ir pasirinkite taikomąją programą, kurią norite panaikinti.
2. Kairiojoje srityje esančioje sekcijoje **tvarkyti** pasirinkite **Ypatybės**.
3. Pasirinkite **Naikinti**, tada pasirinkite **taip** , kad patvirtintumėte, jog norite panaikinti taikomąją programą iš "Azure AD" nuomotojo.

Daugiau informacijos apie tai, kaip panaikinti programėlę, rasite " [QuickStart": taikomosios programos naikinimas "Azure Active Directory" ("AZURE AD") nuomotojuje](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

"PowerShell", " [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) " cmdlet pašalina taikomosios programos tarpinio serverio konfigūracijas iš konkrečios programos "Azure Active Directory" ir gali visiškai panaikinti taikomąją programą, jei nurodyta.

Galite **atkurti panaikintą taikomąją programą** naudodami "PowerShell". Nustačius programą, kurią norite atkurti, galite ją atkurti naudodami [atkurti – Azureadnaikintiprograma](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
