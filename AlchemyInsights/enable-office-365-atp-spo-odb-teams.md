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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709915"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="96fe6-102">"Office 365" išplėstinės grėsmių apsaugos "SharePoint Online", "OneDrive" ir "Microsoft teams" įgalinimas</span><span class="sxs-lookup"><span data-stu-id="96fe6-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="96fe6-103">Eikite į https://protection.office.com ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="96fe6-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="96fe6-104">Pasirinkite **grėsmių valdymo**  >  **strategijos**  >  **saugos priedai**.</span><span class="sxs-lookup"><span data-stu-id="96fe6-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="96fe6-105">Pasirinkite **įjungti "SharePoint", "OneDrive" ir "Microsoft teams" ATP**, tada spustelėkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="96fe6-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="96fe6-106">Rekomenduojama Kaip visuotinis administratorius arba "SharePoint Online" administratorius, paleiskite [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet, naudodami parametrą **Disallowinfectedfiledownload** ( *teisinga*).</span><span class="sxs-lookup"><span data-stu-id="96fe6-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="96fe6-107">Rekomenduojama [Nustatykite](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) aptiktų failų įspėjimus.</span><span class="sxs-lookup"><span data-stu-id="96fe6-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="96fe6-108">ATP bus nNorėdami nuskaityti kiekvieną failą "SharePoint Online", "OneDrive" arba "Microsoft teams".</span><span class="sxs-lookup"><span data-stu-id="96fe6-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="96fe6-109">Failai nuskaitomi asinchroniškai, taikant procesą, kuris naudoja bendro naudojimo ir svečių veiklos įvykius, kartu su "Smart euristiką" ir grėsmių signalais, kad identifikuotumėte kenkėjiškus failus.</span><span class="sxs-lookup"><span data-stu-id="96fe6-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="96fe6-110">Ieškokite " [SharePoint", "OneDrive" ir "Microsoft teams" ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="96fe6-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>