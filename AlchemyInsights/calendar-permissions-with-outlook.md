---
title: Kalendoriaus teisės
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862174"
---
# <a name="calendar-permissions"></a>Kalendoriaus teisės

Vartotojai gali pakeisti savo kalendoriaus teises naudodami "Outlook" žiniatinklyje ar kituose klientuose, bet kaip administratorius, kurį taip pat gali reikėti ištirti.  
Su "Exchange PowerShell" cmdlet parodys vartotojo kalendoriaus teises:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Norėdami pamatyti daugiau informacijos, žr.:

- [Get-MailboxFolderPermission (Get-MailboxFolderPermission)](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission Set-MailboxFolderPermission Nustatyti MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Pridėti MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalendoriaus teisės naudojamos bendrinant kalendorius, norint pamatyti daugiau informacijos apie "Outlook" kalendoriaus bendrinimą, žr.

- [„Outlook“ kalendoriaus bendrinimas su kitais žmonėmis](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalendoriaus bendrinimas internetinėje "Outlook" verslui](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Norėdami pašalinti kalendoriaus teisių triktis, galite naudoti [palaikymo ir atkūrimo asistento](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) įrankį.