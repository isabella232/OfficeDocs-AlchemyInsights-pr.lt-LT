---
title: „Microsoft 365“ grupei siunčiamus pranešimus gauna ne visi nariai
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823795"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="fd19f-102">„Microsoft 365“ grupei siunčiamus pranešimus gauna ne visi nariai</span><span class="sxs-lookup"><span data-stu-id="fd19f-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="fd19f-103">Įsitikinkite, kad visi grupės nariai užsiprenumeravo gauti el. laiškus.</span><span class="sxs-lookup"><span data-stu-id="fd19f-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="fd19f-104">Žr. [Stebėti grupę programoje „Outlook“](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="fd19f-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="fd19f-105">Norėdami patikrinti narių, kurie užsiprenumeravo grupės el. laiškus, pranešimų būseną, paleiskite toliau pateiktą komandą naudodami [„EXO PowerShell“](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="fd19f-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="fd19f-106">Naudodami šią „EXO PowerShell“ komandą sukonfigūruokite, kad visi grupės nariai savo aplankuose Gauta gautų el. laiškus, siunčiamus „Microsoft 365“ grupei:</span><span class="sxs-lookup"><span data-stu-id="fd19f-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="fd19f-107">Toliau pateikiami pavyzdžiai.</span><span class="sxs-lookup"><span data-stu-id="fd19f-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`