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
# <a name="unable-to-change-username"></a><span data-ttu-id="df282-102">Neįmanoma pakeisti vartotojo vardo</span><span class="sxs-lookup"><span data-stu-id="df282-102">Unable to change UserName</span></span>

<span data-ttu-id="df282-103">Kai kuriais atvejais UPN (UserPrincipalName) pakeitimai nėra platinami į nuotolinių išteklių saugyklą.</span><span class="sxs-lookup"><span data-stu-id="df282-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="df282-104">Galite gauti tikrinimo klaidų "Office 365" portale arba negalite pakeisti vartotojo vardo arba el. pašto adreso.</span><span class="sxs-lookup"><span data-stu-id="df282-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="df282-105">Norėdami išspręsti šią problemą, rankiniu būdu nustatyti UserPrincipalName naudojant šią "PowerShell" komandą.</span><span class="sxs-lookup"><span data-stu-id="df282-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="df282-106">**Pavyzdys: vartotojo pervardijimas**</span><span class="sxs-lookup"><span data-stu-id="df282-106">**Example: Rename a user**</span></span>

<span data-ttu-id="df282-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="df282-107">PowerShellCopy</span></span>

<span data-ttu-id="df282-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" - NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="df282-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="df282-109">Ši komanda pervardija davidc@contoso.com į davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="df282-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="df282-110">Daugiau informacijos ieškokite [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="df282-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>