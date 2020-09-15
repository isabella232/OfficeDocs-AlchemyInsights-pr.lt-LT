---
title: Nepavyksta atidaryti naudojant "Explorer"
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694464"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="a2fb0-102">Nepavyksta atidaryti naudojant "Explorer"</span><span class="sxs-lookup"><span data-stu-id="a2fb0-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="a2fb0-103">Jei **Atidaryti naudojant "Explorer"** arba **rodinį failų naršyklėje** neveikia, įsitikinkite, kad "WebClient" tarnyba nustatyta **veikti** , atlikdami toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="a2fb0-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="a2fb0-104">Pavyzdžiui, gali reikėti ilgai atidaryti "SharePoint" arba "OneDrive" biblioteką, kai tarnyba nepaleista.</span><span class="sxs-lookup"><span data-stu-id="a2fb0-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="a2fb0-105">"Windows" ieškos lauke įveskite vykdyti, pasirinkite paleisti kompiuterio taikomąją programą, įveskite Services. msc, tada pasirinkite **įvesti**.</span><span class="sxs-lookup"><span data-stu-id="a2fb0-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="a2fb0-106">Slinkite žemyn iki žiniatinklio kliento tarnybos ir patikrinkite stulpelį **Būsena** .</span><span class="sxs-lookup"><span data-stu-id="a2fb0-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="a2fb0-107">Jei WebClient tarnybos būsena **nepaleista**, dukart spustelėkite tarnybą, spustelėkite **pradėti**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="a2fb0-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="a2fb0-108">Įjunkite paslaugą, jei reikia, lauke **Paleisties tipas** pasirinkite **Rankinis** arba **Automatinis** .</span><span class="sxs-lookup"><span data-stu-id="a2fb0-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a2fb0-109">Norėdami šalinti problemas, atidaromas failų naršyklėje, žiūrėkite [Atidaryti naudojant "Explorer"](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="a2fb0-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="a2fb0-110">Peržiūrėkite sinchronizavimą kaip geresnę alternatyva: [Sinchronizuokite "SharePoint" failus su naujuoju "OneDrive" sinchronizavimo klientu](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a2fb0-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

