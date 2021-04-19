---
title: PST importavimo problemų šalinimas
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
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826171"
---
# <a name="troubleshooting-pst-import-issues"></a>PST importavimo problemų šalinimas

- Jei importuojate iš „Outlook“ kliento, žr. [„Outlook“ .pst failo importavimo problemų sprendimas](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Jei naudojate importavimo tarnybą ir ji užstringa, atminkite, kad kiekvienas PST failas, kurį nusiunčiate į „Azure“ saugyklos vietą, neturėtų būti didesnis nei 20 GB. PST failai, didesni nei 20 GB, gali paveikti PST importavimo procesą.

- Jei norite patikrinti konkrečios importavimo užduoties būseną, galite naudoti [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Išsamią informaciją apie importavimo tarnybą žr. [Organizacijos PST failų importavimo apžvalga](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
