---
title: Siuntėjas negauna laiškų, siunčiamų "Microsoft 365" grupei
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871968"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="12c20-102">Siuntėjas negauna laiškų, siunčiamų "Microsoft 365" grupei</span><span class="sxs-lookup"><span data-stu-id="12c20-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="12c20-103">Pagal numatytuosius, el. laiško siuntėjui "Microsoft 365" grupei negauna pranešimo kopijos savo aplanke Gauta, net jei siuntėjas yra grupės narys.</span><span class="sxs-lookup"><span data-stu-id="12c20-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="12c20-104">Naudokite šią "EXO PowerShell" komandą, kad siuntėjas gautų kiekvieno elektroninio pašto, kurį jie siunčia "Microsoft" 365 grupei, kopiją:</span><span class="sxs-lookup"><span data-stu-id="12c20-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="12c20-105">Norėdami įjungti visų pašto dėžučių parametrą vienu metu:</span><span class="sxs-lookup"><span data-stu-id="12c20-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="12c20-106">**Pastaba** Šio parametro keitimas užtrunka iki valandos, kad įsigaliotų.</span><span class="sxs-lookup"><span data-stu-id="12c20-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>