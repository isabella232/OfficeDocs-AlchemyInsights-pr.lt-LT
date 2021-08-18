---
title: "\"Office 365 ATP\" SharePoint, \"\"OneDrive\"\" ir \"Microsoft Teams"
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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332167"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>"Microsoft" sargybos Office 365, SharePoint, "OneDrive" ir Microsoft Teams

1. Eikite https://protection.office.com ir prisijunkite.
2. Pasirinkite **Grėsmių**  >  **valdymo strategija** Seifas  >  **priedai.**
3. Pasirinkite **Įjungti sargybą Office 365, SharePoint, "OneDrive"** ir Microsoft Teams , tada spustelėkite **Įrašyti**.
4. (Rekomenduojama) Kaip visuotinis administratorius arba "SharePoint Online" administratorius, paleiskite ["Cmdlet" Set-SPOTenant,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) naudodami **parametrą DisallowInfectedFileDownload,** nustatytą *kaip true*.
5. (Rekomenduojama) [Nustatykite aptiktų](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) failų įspėjimus.

**Pastaba:**"Microsoft" Office 365, skirta "Office 365", neskaitys kiekvieno "SharePoint Online", ""OneDrive"" arba "Microsoft Teams". Failai nuskaitomi asinchroniškai, naudojant bendrinimo ir svečio veiklos įvykius, kartu su išmaniais heuristics ir grėsmių signalais kenkėjiškiems failams identifikuoti. Žr. ["Microsoft" sargybos Office 365, SharePoint, "OneDrive" ir Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
