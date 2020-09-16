---
title: Kalendoriaus teisės
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748801"
---
# <a name="calendar-permissions"></a>Kalendoriaus teisės

Vartotojai gali keisti savo kalendoriaus teises su "Outlook" žiniatinklyje ar kituose klientuose, bet kaip administratorius gali tekti taip pat atlikti tyrimus.  
Naudojant "Exchange PowerShell" cmdlet, bus rodoma vartotojo kalendoriaus teisė:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Daugiau informacijos rasite toliau:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Įtraukti MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendoriaus teisės naudojamos kalendorių dalinimosi srityje, kad pamatytumėte daugiau informacijos apie "Outlook" kalendoriaus bendrą naudojimą, peržiūrėkite šiuos straipsnius:

- [„Outlook“ kalendoriaus bendrinimas su kitais žmonėmis](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendoriaus bendrinimas internetinėje "Outlook" verslui](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Norėdami šalinti kalendoriaus teises, galite naudoti [palaikymo ir atkūrimo asistento](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) įrankį.