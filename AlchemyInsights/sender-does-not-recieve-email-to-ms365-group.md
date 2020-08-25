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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Siuntėjas negauna laiškų, siunčiamų "Microsoft 365" grupei

Pagal numatytuosius, el. laiško siuntėjui "Microsoft 365" grupei negauna pranešimo kopijos savo aplanke Gauta, net jei siuntėjas yra grupės narys.

Naudokite šią "EXO PowerShell" komandą, kad siuntėjas gautų kiekvieno elektroninio pašto, kurį jie siunčia "Microsoft" 365 grupei, kopiją:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Norėdami įjungti visų pašto dėžučių parametrą vienu metu:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Pastaba** Šio parametro keitimas užtrunka iki valandos, kad įsigaliotų.