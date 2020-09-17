---
title: 929 aplanko Gauta taisyklės, skirtos "Defecttransport" taisyklėms
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778699"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="cb574-102">Pašto srauto taisyklės (taip pat vadinamos transportavimo taisyklėmis)</span><span class="sxs-lookup"><span data-stu-id="cb574-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="cb574-103">Bendroji pašto srauto taisyklių apžvalga: [pašto srauto taisyklės (transportavimo taisyklės) "Exchange Online](https://technet.microsoft.com/library/jj919238.aspx) "</span><span class="sxs-lookup"><span data-stu-id="cb574-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="cb574-104">Pašto srauto taisyklių nustatymas: [pašto srauto taisyklės procedūros "Exchange Online](https://technet.microsoft.com/library/dn600436.aspx) "</span><span class="sxs-lookup"><span data-stu-id="cb574-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="cb574-105">Pašto srauto taisyklių kūrimas, modifikavimas ir naikinimas: [pašto srauto taisyklių valdymas](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="cb574-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="cb574-106">Taip pat galite tvarkyti pašto srauto taisykles "Exchange Online" "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="cb574-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="cb574-107">Daugiau informacijos rasite [get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (rodinys), [New-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (kurti), [Remove-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (panaikinti), [Set-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modifikuoti esamus), [išjungti-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (išjungti esamą) ir [įgalinti-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (įgalinti esamą).</span><span class="sxs-lookup"><span data-stu-id="cb574-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="cb574-108">Papildomos pašto srauto taisyklės cmdlet: [get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (sąrašo galimi veiksmai), [get-Transportrulepreatate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (sąrašas galimos sąlygos ir išimtys), [Export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (eksporto taisyklės) ir [Import-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (importo taisyklės).</span><span class="sxs-lookup"><span data-stu-id="cb574-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
