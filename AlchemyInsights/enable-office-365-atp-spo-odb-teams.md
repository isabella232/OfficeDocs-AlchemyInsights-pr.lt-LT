---
title: Įgalinti "Office 365" ATP SharePoint, "OneDrive" ir "Microsoft" komandos
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403041"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Įjungti Office 365 Išplėstinė grėsmę apsaugos SharePoint internete, "OneDrive" ir "Microsoft" komandos

1. Eikite į https://protection.office.com ir prisijunkite.
2. Pasirinkti **grėsmės valdymo** > **politikos** > **Saugos priedus**.
3. Pasirinkite **įjungti ATP SharePoint, "OneDrive", ir "Microsoft" komandomis**, o tada spustelėkite **įrašyti**.
4. (Rekomenduojama) Kaip visuotinis administratorius arba SharePoint Online administratorius, paleiskite [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet **DisallowInfectedFileDownload** parametras nustatytas kaip *true*.
5. (Rekomenduojama) [Nustatyti įspėjimus](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) aptikti failai.

> [!NOTE]
> ATP bus NTT nuskaityti kiekvieną vieną failą į SharePoint Online, OneDrive arba "Microsoft" Teams. Failai yra nuskaitomi asynchronicznie, per procesą, kuris naudoja pasidalijimo ir svečių aktyvumas renginiai, kartu su protingas Euristika ir pavojaus signalus kenkėjiškų failų. Matyti [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).