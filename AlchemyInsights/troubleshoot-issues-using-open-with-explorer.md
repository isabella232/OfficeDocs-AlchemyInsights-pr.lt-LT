---
title: Problemų šalinimas naudojant "Open with Explorer"
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742741"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="1e46f-102">"Open with Explorer" problemų sprendimas</span><span class="sxs-lookup"><span data-stu-id="1e46f-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="1e46f-103">Išspręskite bendrąsias problemas atidarydami "SharePoint" arba "OneDrive" dokumentų biblioteką naudodami komandą **Atidaryti naudojant "Internet Explorer"** :</span><span class="sxs-lookup"><span data-stu-id="1e46f-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="1e46f-104">Naudokite Internet Explorer 10 arba Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="1e46f-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="1e46f-105">**Atidaryti naudojant "Explorer** " nesuderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kt.</span><span class="sxs-lookup"><span data-stu-id="1e46f-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="1e46f-106">**Atidaryti naudojant Explorer** yra išjungtas visose naršyklėse, išskyrus Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="1e46f-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="1e46f-107">Šiuolaikinės "SharePoint" bibliotekų patirties negalima **Atidaryti naudojant "Explorer** ".</span><span class="sxs-lookup"><span data-stu-id="1e46f-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="1e46f-108">Vietoj to naudokite **rodinį failų naršyklėje** .</span><span class="sxs-lookup"><span data-stu-id="1e46f-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="1e46f-109">Pasirinkite **Peržiūrėti parinkčių** \> **rodinį failų naršyklėje**.</span><span class="sxs-lookup"><span data-stu-id="1e46f-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="1e46f-110">"File Explorer" rodinys nesuderinamas su "Microsoft Edge", "Google Chrome", "Firefox" ir kitomis.</span><span class="sxs-lookup"><span data-stu-id="1e46f-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="1e46f-111">**Peržiūrėti failų naršyklėje** galima tik "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="1e46f-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="1e46f-112">Įsitikinkite, kad veikia WebClient tarnyba.</span><span class="sxs-lookup"><span data-stu-id="1e46f-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="1e46f-113">"Windows" ieškos lauke įveskite paleisti, pasirinkite paleisti darbalaukio programėlę, įveskite Services. msc, tada paspauskite ENTER.</span><span class="sxs-lookup"><span data-stu-id="1e46f-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="1e46f-114">Slinkite žemyn į WebClient tarnybą ir įsitikinkite, kad **būsenos** stulpelyje rodomas "veikia".</span><span class="sxs-lookup"><span data-stu-id="1e46f-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="1e46f-115">Jei ne, dukart spustelėkite tarnybą, spustelėkite **pradėtiteir**tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="1e46f-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="1e46f-116">( **Paleisties tipo** lauke gali reikėti pirmiausia įjungti paslaugą, pasirinkus **Rankinis** arba **Automatinis** .)</span><span class="sxs-lookup"><span data-stu-id="1e46f-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1e46f-117">Bibliotekos atidarymas failų naršyklėje yra parankus, jei reikia vieną kartą kopijuoti arba perkelti kelis failus ir aplankus, bet jei norite reguliariai dirbti bibliotekoje, rekomenduojame ją sinchronizuoti.</span><span class="sxs-lookup"><span data-stu-id="1e46f-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="1e46f-118">Norėdami išspręsti problemas, atidarymo failų naršyklėje, pamatyti [atidaryti naršyklėje](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="1e46f-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="1e46f-119">Informacijos apie sinchronizavimo nustatymą ieškokite [SharePoint failų sinchronizavimas su naujuoju "OneDrive" sinchronizavimo klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="1e46f-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="1e46f-120">Žiūrėkite straipsnį, [kaip naudoti komandą "Open with Explorer" spręsti problemas, SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="1e46f-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

