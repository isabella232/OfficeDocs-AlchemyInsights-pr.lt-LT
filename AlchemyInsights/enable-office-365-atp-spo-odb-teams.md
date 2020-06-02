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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506926"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="dab54-102">"Office 365" išplėstinės apsaugos nuo grėsmių įgalinimas "SharePoint Online", "OneDrive" ir "Microsoft Teams"</span><span class="sxs-lookup"><span data-stu-id="dab54-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="dab54-103">Eikite https://protection.office.com ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="dab54-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="dab54-104">Pasirinkite **Grėsmių valdymo**  >  **strategijos**  >  **saugūs priedai**.</span><span class="sxs-lookup"><span data-stu-id="dab54-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="dab54-105">Pasirinkite **Įjungti "SharePoint", "OneDrive" ir "Microsoft Teams" ATP,** tada spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="dab54-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="dab54-106">(Rekomenduojama) Kaip visuotinis administratorius arba "SharePoint Online" administratorius, vykdykite [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet su **parametru NeleistiInfectedFileDownload** nustatyta *kaip teisinga*.</span><span class="sxs-lookup"><span data-stu-id="dab54-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="dab54-107">(Rekomenduojama) Nustatyti aptiktų [failų įspėjimus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)</span><span class="sxs-lookup"><span data-stu-id="dab54-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="dab54-108">ATP nuskaitys kiekvieną failą "SharePoint Online", "OneDrive" arba "Microsoft Teams".</span><span class="sxs-lookup"><span data-stu-id="dab54-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="dab54-109">Failai nuskaitomi asinchroniškai, naudojant procesą, kuris naudoja bendrinimo ir svečių veiklos įvykius, taip pat išmaniuosius euristikus ir grėsmės signalus kenkėjiškiems failams identifikuoti.</span><span class="sxs-lookup"><span data-stu-id="dab54-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="dab54-110">Peržiūrėkite ["SharePoint", "OneDrive" ir "Microsoft Teams" ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="dab54-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>