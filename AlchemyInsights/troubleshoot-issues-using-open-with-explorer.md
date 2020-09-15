---
title: Trikčių šalinimas naudojant "Explorer"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659066"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="650e6-102">Su naršykle atidarytų problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="650e6-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="650e6-103">Išspręskite įprastas problemas, susijusias su "SharePoint" arba "OneDrive" dokumentų bibliotekos atidarymu naudodami komandą **Atidaryti naudojant Explorer** :</span><span class="sxs-lookup"><span data-stu-id="650e6-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="650e6-104">Naudokite "Internet Explorer 10" arba "Internet Explorer 11".</span><span class="sxs-lookup"><span data-stu-id="650e6-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="650e6-105">**Atidaryti naudojant "Explorer** " nesuderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kt.</span><span class="sxs-lookup"><span data-stu-id="650e6-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="650e6-106">**Atidaryti naudojant "Explorer"** išjungta visose naršyklėse, išskyrus "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="650e6-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="650e6-107">**Atidaryti naudojant "Explorer"** negalima šiuolaikinėje "SharePoint" bibliotekų srityje.</span><span class="sxs-lookup"><span data-stu-id="650e6-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="650e6-108">Vietoj to naudokite **rodinį failų naršyklėje** .</span><span class="sxs-lookup"><span data-stu-id="650e6-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="650e6-109">Pasirinkite **Peržiūrėti parinkčių** \> **rodinį failų naršyklėje**.</span><span class="sxs-lookup"><span data-stu-id="650e6-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="650e6-110">Rodinys failų naršyklėje nesuderinamas su "Microsoft Edge", "Google Chrome", "Firefox" ir kitais.</span><span class="sxs-lookup"><span data-stu-id="650e6-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="650e6-111">**Peržiūrėti failų naršyklėje** galima tik naudojant "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="650e6-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="650e6-112">Įsitikinkite, kad veikia WebClient tarnyba.</span><span class="sxs-lookup"><span data-stu-id="650e6-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="650e6-113">"Windows" ieškos lauke įveskite vykdyti, pasirinkite paleisti kompiuterio taikomąją programą, įveskite Services. msc, tada paspauskite klavišą "įvesti".</span><span class="sxs-lookup"><span data-stu-id="650e6-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="650e6-114">Slinkite žemyn iki "WebClient" tarnybos ir įsitikinkite, kad stulpelyje **Būsena** rodoma "veikia".</span><span class="sxs-lookup"><span data-stu-id="650e6-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="650e6-115">Jei ne, dukart spustelėkite tarnybą, spustelėkite **pradėti**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="650e6-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="650e6-116">(Pirmiausia gali reikėti įgalinti paslaugą, lauke **Paleisties tipas** pasirinkę **Rankinis** arba **Automatinis** .)</span><span class="sxs-lookup"><span data-stu-id="650e6-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="650e6-117">Jei norite, kad būtų galima kopijuoti arba perkelti kelis failus ir aplankus, galite atidaryti biblioteką failų naršyklėje, bet jei norite reguliariai dirbti bibliotekoje, rekomenduojame ją sinchronizuoti.</span><span class="sxs-lookup"><span data-stu-id="650e6-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="650e6-118">Norėdami šalinti problemas, atidaromas failų naršyklėje, žiūrėkite [Atidaryti naudojant "Explorer"](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="650e6-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="650e6-119">Informacijos apie sinchronizavimo nustatymą ieškokite ["SharePoint" failų sinchronizavimas naudojant naująjį "OneDrive" sinchronizavimo klientą](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="650e6-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="650e6-120">Daugiau informacijos rasite straipsnyje [kaip naudoti komandą Atidaryti naudojant "Explorer", kad išspręstumėte "SharePoint Online" problemas](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="650e6-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

