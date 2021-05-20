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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543936"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="0a42b-102">"Microsoft" sargybos Office 365, SharePoint, "OneDrive" ir Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0a42b-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="0a42b-103">Eikite https://protection.office.com ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="0a42b-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="0a42b-104">Pasirinkite **Grėsmių**  >  **valdymo strategija** Seifas  >  **priedai.**</span><span class="sxs-lookup"><span data-stu-id="0a42b-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="0a42b-105">Pasirinkite **Įjungti sargybą Office 365, SharePoint, "OneDrive" ir Microsoft Teams**, tada spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="0a42b-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="0a42b-106">(Rekomenduojama) Kaip visuotinis administratorius arba "SharePoint Online" administratorius, vykdykite ["cmdlet" Set-SPOTenant,](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) naudodami **parametrą DisallowInfectedFileDownload,** nustatytą *kaip true*.</span><span class="sxs-lookup"><span data-stu-id="0a42b-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="0a42b-107">(Rekomenduojama) [Nustatykite aptiktų](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) failų įspėjimus.</span><span class="sxs-lookup"><span data-stu-id="0a42b-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="0a42b-108">"Microsoft" sargyba Office 365 neskaitys kiekvieno "SharePoint Online", ""OneDrive"" arba "Microsoft Teams" failo.</span><span class="sxs-lookup"><span data-stu-id="0a42b-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="0a42b-109">Failai nuskaitomi asinchroniškai, naudojant bendrinimo ir svečio veiklos įvykius, kartu su išmaniais heuristics ir grėsmių signalais kenkėjiškiems failams identifikuoti.</span><span class="sxs-lookup"><span data-stu-id="0a42b-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="0a42b-110">Žr. ["Microsoft" sargybos Office 365, SharePoint, "OneDrive" ir Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="0a42b-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>