---
title: Atidaryti naudojant "Internet Explorer" trikčių šalinimas
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759302"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="b9a51-102">Problemų su "Internet Explorer" atidaryti</span><span class="sxs-lookup"><span data-stu-id="b9a51-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="b9a51-103">Spręsti bendrąsias problemas su dokumentų biblioteka SharePoint arba "OneDrive" naudodami komandą **Atidaryti naudojant "Internet Explorer"** :</span><span class="sxs-lookup"><span data-stu-id="b9a51-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="b9a51-104">Naudoti Internet Explorer 10 arba Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="b9a51-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="b9a51-105">**Atidaryti naudojant "Internet Explorer"** nėra suderinamas su "Microsoft Edge", "Google Chrome", "Firefox" ir kt.</span><span class="sxs-lookup"><span data-stu-id="b9a51-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="b9a51-106">**Atidaryti naudojant "Internet Explorer"** yra išjungta, visos naršyklės išskyrus Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b9a51-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="b9a51-107">**Atidaryti naudojant Explorer** negalimas šiuolaikinės patirtis SharePoint bibliotekos.</span><span class="sxs-lookup"><span data-stu-id="b9a51-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="b9a51-108">Vietoj to naudokite **Peržiūrėti failų naršyklėje** .</span><span class="sxs-lookup"><span data-stu-id="b9a51-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="b9a51-109">Pasirinkite **Peržiūrėti funkcijos** \> **Peržiūrėti failų naršyklėje**.</span><span class="sxs-lookup"><span data-stu-id="b9a51-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="b9a51-110">Rodyti failų naršyklės nėra suderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kt.</span><span class="sxs-lookup"><span data-stu-id="b9a51-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="b9a51-111">**Rodyti failų naršyklėje** , galite naudotis tik "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="b9a51-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="b9a51-112">Įsitikinkite, kad veikia WebClient tarnyba.</span><span class="sxs-lookup"><span data-stu-id="b9a51-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="b9a51-113">"Windows" ieškos lauke, įrašykite vykdyti, pasirinkite darbalaukio programą, vykdyti, įveskite services.msc ir paspauskite Enter.</span><span class="sxs-lookup"><span data-stu-id="b9a51-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="b9a51-114">Slinkite žemyn iki WebClient tarnybos ir įsitikinkite, kad į **statusas** stulpelyje rodomas "Veikia."</span><span class="sxs-lookup"><span data-stu-id="b9a51-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="b9a51-115">Jei ne, dukart spustelėkite tarnybos, spustelėkite **pradėti**ir tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="b9a51-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b9a51-116">(Gali tekti pirmiausia įjungti paslaugą, pasirinkite **Rankinis** arba **Automatinis** lauke **Paleisties tipas** ).</span><span class="sxs-lookup"><span data-stu-id="b9a51-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b9a51-117">Bibliotekos failų naršyklė yra patogu, jei norite kopijuoti ar perkelti kelis failus ir aplankus, kai, bet jei norite nuolat dirbti bibliotekoje, mes rekomenduojame jį sinchronizuoti.</span><span class="sxs-lookup"><span data-stu-id="b9a51-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="b9a51-118">Triktims atidaryti failų naršyklėje, ieškokite [atidaryti "Internet Explorer"](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b9a51-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b9a51-119">Informacijos apie sinchronizavimo nustatymą ieškokite [sinchronizavimo SharePoint failai su nauja "OneDrive" sinchronizavimo klientas](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b9a51-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="b9a51-120">Žiūrėkite straipsnį [kaip naudoti komandą "atviros su" Explorer "" triktims SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="b9a51-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

