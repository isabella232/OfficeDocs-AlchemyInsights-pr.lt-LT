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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059823"
---
# <a name="troubleshooting-pst-import-issues"></a>PST importavimo problemų šalinimas

- Jei importuojate per patį "Outlook" klientą, [žr. "Outlook" .pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)failo importavimo problemų sprendimas .

- Jei naudojate importavimo tarnybą ir užstringa, atkreipkite dėmesį, kad kiekvienas PST failas, kurį nusiunčiate į "Azure" saugyklos vietą, neturėtų būti didesnis nei 20 GB. PST failai, didesni nei 20 GB, gali turėti įtakos PST importavimo proceso našumui. Daugiau informacijos apie įstrigančių užduočių trikčių [diagnostiką žr. Problemos, kurios turi įtakos PST importavimo uždėjimo vietoms](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Jei norite patikrinti konkrečios importavimo užduoties būseną, naudokite [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Išsamios informacijos apie importavimo tarnybą žr. Organizacijos PST failų [importavimo apžvalga.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
