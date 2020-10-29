---
title: "\"Office 365\" ATP įgalinimas \"SharePoint\", \"OneDrive\" ir \"Microsoft teams\""
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801060"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>"Microsoft Defender", skirto "Office 365" "SharePoint Online", "OneDrive" ir "Microsoft teams" įgalinimas

1. Eikite į https://protection.office.com ir prisijunkite.
2. Pasirinkite **grėsmių valdymo**  >  **strategijos**  >  **saugos priedai** .
3. Pasirinkite **įjungti "SharePoint", "OneDrive" ir "Microsoft teams" ATP** , tada spustelėkite **įrašyti** .
4. Rekomenduojama Kaip visuotinis administratorius arba "SharePoint Online" administratorius, paleiskite [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet, naudodami parametrą **Disallowinfectedfiledownload** ( *teisinga* ).
5. Rekomenduojama [Nustatykite](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) aptiktų failų įspėjimus.

> [!NOTE]
> ATP bus nNorėdami nuskaityti kiekvieną failą "SharePoint Online", "OneDrive" arba "Microsoft teams". Failai nuskaitomi asinchroniškai, taikant procesą, kuris naudoja bendro naudojimo ir svečių veiklos įvykius, kartu su "Smart euristiką" ir grėsmių signalais, kad identifikuotumėte kenkėjiškus failus. Ieškokite " [SharePoint", "OneDrive" ir "Microsoft teams" ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).