---
title: Neįmanoma pakeisti vartotojo vardo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439547"
---
# <a name="unable-to-change-username"></a>Neįmanoma pakeisti vartotojo vardo

Kai kuriais atvejais UPN (UserPrincipalName) pakeitimai nėra platinami į nuotolinių išteklių saugyklą. Galite gauti tikrinimo klaidų "Office 365" portale arba negalite pakeisti vartotojo vardo arba el. pašto adreso. Norėdami išspręsti šią problemą, rankiniu būdu nustatyti UserPrincipalName naudojant šią "PowerShell" komandą.

**Pavyzdys: vartotojo pervardijimas**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" - NewUserPrincipalName "davidchew@contoso.com"

Ši komanda pervardija davidc@contoso.com į davidchew@contoso.com.

Daugiau informacijos ieškokite [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).