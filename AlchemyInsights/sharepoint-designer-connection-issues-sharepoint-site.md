---
title: "\"SharePoint Designer\" prisijungimo problemos"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727179"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="9ecb2-102">"SharePoint Designer" prisijungimo problemos</span><span class="sxs-lookup"><span data-stu-id="9ecb2-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="9ecb2-103">Jei "SharePoint Designer" susiduria su "SharePoint" svetainių prisijungimo problemomis, išbandykite šiuos bendruosius sprendimus.</span><span class="sxs-lookup"><span data-stu-id="9ecb2-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="9ecb2-104">1 veiksmas: patikrinkite, ar "SharePoint Designer 2013" atnaujinama naudojant " [SharePoint Designer" 1 pakeitimų paketą](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [rugpjūčio 2 d., 2016 naujinimą, skirtą "SharePoint Designer 2013"](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="9ecb2-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="9ecb2-105">2 veiksmas: išvalykite vietos talpyklos failus:</span><span class="sxs-lookup"><span data-stu-id="9ecb2-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="9ecb2-106">Uždarykite "SharePoint Designer" 2013.</span><span class="sxs-lookup"><span data-stu-id="9ecb2-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="9ecb2-107">Vietiniame kompiuteryje pašalinkite visus failus, esančius kiekviename iš šių aplankų.</span><span class="sxs-lookup"><span data-stu-id="9ecb2-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="9ecb2-108">%AppData%\microsoft\žiniatinklio serverio Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="9ecb2-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="9ecb2-109">%APPDATA%\Microsoft\SharePoint "Windows" proxyassemblycache</span><span class="sxs-lookup"><span data-stu-id="9ecb2-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="9ecb2-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="9ecb2-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="9ecb2-111">Atidarykite "SharePoint Designer" 2013 ir dar kartą Įeikite į paskyrą, kad sužinotumėte, ar ji veikia.</span><span class="sxs-lookup"><span data-stu-id="9ecb2-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="9ecb2-112">3 veiksmas: [modernaus autentifikavimo įgalinimas "Office 2013" "Windows" įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="9ecb2-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="9ecb2-113">4 veiksmas: administratoriams reikės **leisti pasirinktiniam scenarijui** "SharePoint" administravimo centro parametruose leisti "SharePoint Designer" ryšiui.</span><span class="sxs-lookup"><span data-stu-id="9ecb2-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="9ecb2-114">Daugiau informacijos ieškokite [pasirinktinio scenarijaus leidimas arba neleidimas](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="9ecb2-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


