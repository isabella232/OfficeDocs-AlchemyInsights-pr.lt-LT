---
title: Problemos, SharePoint 7 Windows įrenginių
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125510"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemos, SharePoint 7 Windows įrenginių

Jei dirbdami su "SharePoint" arba ""OneDrive"" gaunate klaidų "Windows 7" kompiuteriuose, jos gali būti susijusios su TLS 1.0/1.1 nutraukimu. Daugiau informacijos rasite:

- [Pasirengimas TLS 1.2 Office 365 ir Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/"Windows 8" klientams turi būti įgalintas TLS1.2. Daugiau informacijos žr. [Autentifikavimo klaidos įvyksta, kai klientas neturi TLS 1.2 palaikymo](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Įdiekite KB3140245 ir sukurkite registro reikšmę. Daugiau informacijos žr. Naujinimas, skirtas [įgalinti TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Windows 7 SP1/"Windows 8" klientai turi užtikrinti, kad būtų įdiegti naujausi TLS šifro paketai. Daugiau informacijos žr. ["Microsoft" saugos patarimo 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


