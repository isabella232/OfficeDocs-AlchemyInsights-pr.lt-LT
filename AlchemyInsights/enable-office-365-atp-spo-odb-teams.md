---
title: "\"Office 365 ATP\", skirtos \"SharePoint\", \"OneDrive\" ir \"Microsoft Teams\", įgalinimas"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703434"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>"Office 365" išplėstinės apsaugos nuo grėsmių įgalinimas "SharePoint Online", "OneDrive" ir "Microsoft Teams"

1. Eikite https://protection.office.com ir prisijunkite.
2. Pasirinkite **Grėsmių valdymo** > **strategijos** > **saugūs priedai**.
3. Pasirinkite **Įjungti "SharePoint", "OneDrive" ir "Microsoft Teams" ATP,** tada spustelėkite **Įrašyti**.
4. (Rekomenduojama) Kaip visuotinis administratorius arba "SharePoint Online" administratorius, vykdykite [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet su **parametru NeleistiInfectedFileDownload** nustatyta *kaip teisinga*.
5. (Rekomenduojama) Nustatyti aptiktų [failų įspėjimus.](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)

> [!NOTE]
> ATP nuskaitys kiekvieną failą "SharePoint Online", "OneDrive" arba "Microsoft Teams". Failai nuskaitomi asinchroniškai, naudojant procesą, kuris naudoja bendrinimo ir svečių veiklos įvykius, taip pat išmaniuosius euristikus ir grėsmės signalus kenkėjiškiems failams identifikuoti. ®r. [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).