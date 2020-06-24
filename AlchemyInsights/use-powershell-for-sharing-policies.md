---
title: "\"PowerShell\" naudojimas bendrinimo strategijoms ir organizacijos ryšiams"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862149"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="fa80b-102">"PowerShell" naudojimas bendrinimo strategijoms ir organizacijos ryšiams</span><span class="sxs-lookup"><span data-stu-id="fa80b-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="fa80b-103">Organizacijos ryšiams peržiūrėkite išsamią sintaksės ir parametrų informaciją: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="fa80b-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="fa80b-104">Norėdami sukurti bendrinimo strategiją, naudokite [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="fa80b-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="fa80b-105">Norėdami [taikyti bendrinimo strategiją pašto dėžutei arba vartotojui,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) turite naudoti [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ir [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) derinį su naujai sukurta strategija.</span><span class="sxs-lookup"><span data-stu-id="fa80b-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="fa80b-106">Norėdami [modifikuoti, išjungti arba pašalinti bendrinimo strategiją,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) turite naudoti [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ir [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="fa80b-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="fa80b-107">**Norėdami visiškai suprasti šią temą, prašome perskaityti:**</span><span class="sxs-lookup"><span data-stu-id="fa80b-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="fa80b-108">Bendrinimas "Exchange Online"</span><span class="sxs-lookup"><span data-stu-id="fa80b-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)