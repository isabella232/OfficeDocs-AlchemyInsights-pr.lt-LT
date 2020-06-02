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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511552"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="c02dd-102">"SharePoint Designer" ryšio problemos</span><span class="sxs-lookup"><span data-stu-id="c02dd-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="c02dd-103">Jei SharePoint Designer kyla ryšio su SharePoint svetainėmis problemų, išbandykite šiuos bendruosius sprendimus.</span><span class="sxs-lookup"><span data-stu-id="c02dd-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="c02dd-104">1 veiksmas: Patikrinkite, ar SharePoint Designer 2013 yra atnaujintas [su SharePoint Designer 1 pakeitimų paketas](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [2016 m. rugpjūčio 2 naujinimas SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="c02dd-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="c02dd-105">2 veiksmas: išvalykite vietinės talpyklos failus:</span><span class="sxs-lookup"><span data-stu-id="c02dd-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="c02dd-106">Uždarykite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c02dd-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="c02dd-107">Vietiniame kompiuteryje pašalinkite visus failus, rastą kiekviename iš šių aplankų.</span><span class="sxs-lookup"><span data-stu-id="c02dd-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="c02dd-108">%APPDATA%\Microsoft\Web serverio plėtiniai\talpykla</span><span class="sxs-lookup"><span data-stu-id="c02dd-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="c02dd-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APP</span><span class="sxs-lookup"><span data-stu-id="c02dd-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="c02dd-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USER</span><span class="sxs-lookup"><span data-stu-id="c02dd-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="c02dd-111">Atidarykite SharePoint Designer 2013 ir dar kartą įveskite abonementą, kad sužinotumėte, ar jis veikia.</span><span class="sxs-lookup"><span data-stu-id="c02dd-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="c02dd-112">3 veiksmas: [Įgalinkite šiuolaikinės autentifikavimas Office 2013 "Windows" įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c02dd-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="c02dd-113">4 veiksmas: Administratoriai turės **leisti pasirinktinį scenarijų** "SharePoint" administravimo centro parametruose, kad "SharePoint Designer" ryšys būtų leidžiamas.</span><span class="sxs-lookup"><span data-stu-id="c02dd-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="c02dd-114">Daugiau informacijos rasite [Pasirinktinio scenarijaus leidimas arba draudimas.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="c02dd-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


