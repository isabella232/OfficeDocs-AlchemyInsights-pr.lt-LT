---
title: Atidaryti naudojant "Explorer" neveikia
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713042"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="e14ed-102">Atidaryti naudojant "Explorer" neveikia</span><span class="sxs-lookup"><span data-stu-id="e14ed-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="e14ed-103">Jei **atidaryti naudojant "Explorer"** arba **peržiūrėti failų naršyklėje** neveikia įsitikinkite, kad WebClient tarnyba nustatyta **kaip veikia** atlikdami toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="e14ed-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="e14ed-104">Pavyzdžiui, gali ilgai užtrukti atidaryti "SharePoint" arba "OneDrive" biblioteką, kai tarnyba neveikia.</span><span class="sxs-lookup"><span data-stu-id="e14ed-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="e14ed-105">"Windows" ieškos lauke įveskite vykdyti, pasirinkite programėlę Paleisti darbalaukį, įveskite services.msc, tada pasirinkite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e14ed-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="e14ed-106">Slinkite žemyn iki WebClient tarnybos ir patikrinkite stulpelį **Būsena.**</span><span class="sxs-lookup"><span data-stu-id="e14ed-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="e14ed-107">Jei WebClient tarnybos būsena **neveikia**, dukart spustelėkite tarnybą, spustelėkite **pradėti**, ir tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="e14ed-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e14ed-108">Jei reikia, įjunkite tarnybą lauke **Paleisties tipas** pasirinkdami **Rankinis** arba **Automatinis.**</span><span class="sxs-lookup"><span data-stu-id="e14ed-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e14ed-109">Norėdami šalinti failų naršyklės atidarymo triktis, [žr.](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="e14ed-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e14ed-110">Naršykite sinchronizavimą kaip geresnę alternatyvą: [sinchronizuokite "SharePoint" failus su nauju "OneDrive" sinchronizavimo klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e14ed-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

