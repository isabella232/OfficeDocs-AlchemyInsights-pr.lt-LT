---
title: „PowerShell“ naudojimas strategijų bendrinimui ir organizacijos ryšiams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998475"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>„PowerShell“ naudojimas strategijų bendrinimui ir organizacijos ryšiams


Organizacijos ryšiams peržiūrėkite išsamią sintaksę ir parametrų informaciją, skirtą funkcijoms: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) IR [Remove-OrganizationRelation](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Norėdami sukurti bendrinimo strategiją, naudokite funkciją [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Norėdami [taikyti bendrinimo strategiją pašto dėžutei arba vartotojui](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), turite naudoti [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ir [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) derinį su naujai sukurta strategija. Norėdami [keisti, išjungti arba pašalinti bendrinimo strategiją](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), turite naudoti funkcijas [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ir [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Kad visiškai suprastumėte šią temą, perskaitykite:**

[Bendrinimas „Exchange Online“](https://docs.microsoft.com/exchange/sharing/sharing)