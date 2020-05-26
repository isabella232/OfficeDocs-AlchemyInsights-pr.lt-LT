---
title: Blokuoti atsisiuntimą bendrinant saitus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358038"
---
# <a name="block-download-on-sharing-links"></a>Blokuoti atsisiuntimą bendrinant saitus

**Blokuoti atsisiuntimą** galima **tik peržiūrėti saitus** su "Office" dokumentais. Pasirinkus šią parinktį, žmonės, kurie gauna prieigą prie failo per sukurtą saitą, nematys failo atsisiuntimo, spausdinimo ar kopijavimo parinkčių.

Administratoriai gali kontroliuoti, ar parametras "blokuoti atsisiuntimą" rodomas tik "Office" failams, ar ne, pakeisdami `BlockDownloadLinksFileType` [set-SPOTenant arba Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) "PowerShell" cmdlet parametrą. [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)
