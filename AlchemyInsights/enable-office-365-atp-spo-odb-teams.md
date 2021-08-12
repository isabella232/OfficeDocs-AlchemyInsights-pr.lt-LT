---
title: "\"Office 365\" ATP įgalinkite SharePoint, \"OneDrive\" ir Microsoft Teams"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964641"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>"Microsoft" sargybos Office 365, SharePoint, "OneDrive" ir Microsoft Teams

1. Eikite https://protection.office.com ir prisijunkite.
2. Pasirinkite **Grėsmių**  >  **valdymo strategija** Seifas  >  **priedai.**
3. Pasirinkite **Įjungti sargybą Office 365, SharePoint, "OneDrive" ir Microsoft Teams**, tada spustelėkite **Įrašyti**.
4. (Rekomenduojama) Kaip visuotinis administratorius arba "SharePoint Online" administratorius, vykdykite ["cmdlet" Set-SPOTenant,](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) naudodami **parametrą DisallowInfectedFileDownload,** nustatytą *kaip true*.
5. (Rekomenduojama) [Nustatykite aptiktų](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) failų įspėjimus.

> [!NOTE]
> "Microsoft" sargyba Office 365 neskaitys kiekvieno "SharePoint Online", ""OneDrive"" arba "Microsoft Teams" failo. Failai nuskaitomi asinchroniškai, naudojant bendrinimo ir svečio veiklos įvykius, kartu su išmaniais heuristics ir grėsmių signalais kenkėjiškiems failams identifikuoti. Žr. ["Microsoft" sargybos Office 365, SharePoint, "OneDrive" ir Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)