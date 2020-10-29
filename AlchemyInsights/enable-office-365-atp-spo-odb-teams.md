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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3555c-102">"Microsoft Defender", skirto "Office 365" "SharePoint Online", "OneDrive" ir "Microsoft teams" įgalinimas</span><span class="sxs-lookup"><span data-stu-id="3555c-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="3555c-103">Eikite į https://protection.office.com ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="3555c-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="3555c-104">Pasirinkite **grėsmių valdymo**  >  **strategijos**  >  **saugos priedai** .</span><span class="sxs-lookup"><span data-stu-id="3555c-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="3555c-105">Pasirinkite **įjungti "SharePoint", "OneDrive" ir "Microsoft teams" ATP** , tada spustelėkite **įrašyti** .</span><span class="sxs-lookup"><span data-stu-id="3555c-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="3555c-106">Rekomenduojama Kaip visuotinis administratorius arba "SharePoint Online" administratorius, paleiskite [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet, naudodami parametrą **Disallowinfectedfiledownload** ( *teisinga* ).</span><span class="sxs-lookup"><span data-stu-id="3555c-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="3555c-107">Rekomenduojama [Nustatykite](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) aptiktų failų įspėjimus.</span><span class="sxs-lookup"><span data-stu-id="3555c-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="3555c-108">ATP bus nNorėdami nuskaityti kiekvieną failą "SharePoint Online", "OneDrive" arba "Microsoft teams".</span><span class="sxs-lookup"><span data-stu-id="3555c-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="3555c-109">Failai nuskaitomi asinchroniškai, taikant procesą, kuris naudoja bendro naudojimo ir svečių veiklos įvykius, kartu su "Smart euristiką" ir grėsmių signalais, kad identifikuotumėte kenkėjiškus failus.</span><span class="sxs-lookup"><span data-stu-id="3555c-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="3555c-110">Ieškokite " [SharePoint", "OneDrive" ir "Microsoft teams" ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="3555c-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>