---
title: Pranešimus, išsiųstus "Microsoft 365" grupei, gauna ne visi nariai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: lt-LT
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051502"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="f3960-102">Pranešimus, išsiųstus "Microsoft 365" grupei, gauna ne visi nariai</span><span class="sxs-lookup"><span data-stu-id="f3960-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="f3960-103">Įsitikinkite, kad visi grupės nariai užsiprenumeravote gauti el. laiškus.</span><span class="sxs-lookup"><span data-stu-id="f3960-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="f3960-104">Žiūrėkite [Stebėti grupę programoje "Outlook".](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)</span><span class="sxs-lookup"><span data-stu-id="f3960-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="f3960-105">Norėdami patikrinti pranešimo būseną narių, kurie užsiprenumeravote grupės el. laiškus, vykdykite šią komandą ["EXO PowerShell":](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="f3960-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`