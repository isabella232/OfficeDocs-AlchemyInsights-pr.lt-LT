---
title: "\"SharePoint Designer\" ryšio problemos"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051721"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="e4309-102">"SharePoint Designer" ryšio problemos</span><span class="sxs-lookup"><span data-stu-id="e4309-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="e4309-103">Jei SharePoint Designer susiduria su "SharePoint" svetainių ryšio problemomis, išbandykite toliau nurodytus bendruosius sprendimus.</span><span class="sxs-lookup"><span data-stu-id="e4309-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="e4309-104">1 veiksmas: patikrinkite, ar SharePoint Designer 2013 yra atnaujinama naudojant [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [rugpjūčio 2, 2016 naujinimas SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="e4309-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="e4309-105">2 veiksmas: išvalykite vietos talpyklos failus:</span><span class="sxs-lookup"><span data-stu-id="e4309-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="e4309-106">Uždarykite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="e4309-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="e4309-107">Vietiniame kompiuteryje, pašalinkite visus failus, rasti kiekviename iš šių aplankų.</span><span class="sxs-lookup"><span data-stu-id="e4309-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="e4309-108">%APPDATA%\Microsoft\Web serverio Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="e4309-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="e4309-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="e4309-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="e4309-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="e4309-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="e4309-111">Atidarykite "SharePoint Designer 2013" ir dar kartą įveskite paskyrą, kad sužinotumėte, ar ji veikia.</span><span class="sxs-lookup"><span data-stu-id="e4309-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="e4309-112">3 veiksmas: [įgalinkite šiuolaikinės autentifikavimo Office 2013 "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e4309-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="e4309-113">4 veiksmas: administratoriai turės **leisti pasirinktinį scenarijų** SharePoint administravimo centro parametruose leisti SharePoint Designer ryšį.</span><span class="sxs-lookup"><span data-stu-id="e4309-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="e4309-114">Norėdami gauti daugiau informacijos, žiūrėkite [leisti arba neleisti pasirinktinio scenarijaus](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="e4309-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


