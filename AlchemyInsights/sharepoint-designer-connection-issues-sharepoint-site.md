---
title: SharePoint Designer ryšio problemas
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840559"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="731e9-102">SharePoint Designer ryšio problemas</span><span class="sxs-lookup"><span data-stu-id="731e9-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="731e9-103">Jei SharePoint Designer patiria ryšio problemas prie SharePoint svetainės, pabandykite šiuos bendrosios sprendimus.</span><span class="sxs-lookup"><span data-stu-id="731e9-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="731e9-104">1 veiksmas: Patikrinkite, ar kad SharePoint Designer 2013 m. atnaujinti [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [2 rugpjūtis 2016 atnaujinti SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="731e9-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="731e9-105">2 veiksmas: Išvalykite vietinės talpyklos failus:</span><span class="sxs-lookup"><span data-stu-id="731e9-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="731e9-106">Uždarykite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="731e9-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="731e9-107">Vietiniame kompiuteryje, pašalinkite visus failus, randami kiekviename iš šių aplankų.</span><span class="sxs-lookup"><span data-stu-id="731e9-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="731e9-108">%AppData%\Microsoft\Web serveris Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="731e9-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="731e9-109">%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="731e9-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="731e9-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="731e9-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="731e9-111">Atidarykite SharePoint Designer 2013 ir įvesti sąskaitą, dar kartą Norėdami pamatyti, jei ji veikia.</span><span class="sxs-lookup"><span data-stu-id="731e9-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="731e9-112">3 veiksmas: [įgalinti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="731e9-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="731e9-113">4 žingsnis: Administratoriams reikės **Leisti Custom scenarijų** SharePoint administravimo centro parametrai leisti SharePoint Designer ryšį.</span><span class="sxs-lookup"><span data-stu-id="731e9-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="731e9-114">Žr [leisti arba neleisti pasirinktinį scenarijų](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="731e9-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


