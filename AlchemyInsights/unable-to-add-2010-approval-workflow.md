---
title: Neįmanoma įtraukti 2010 m. patvirtinimo darbo eigos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582855"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="ae517-102">Neįmanoma įtraukti 2010 m. patvirtinimo darbo eigos</span><span class="sxs-lookup"><span data-stu-id="ae517-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="ae517-103">Microsoft SharePoint svetainių rinkinyje negalite įtraukti visuotinai pakartotinai naudojamos darbo eigos (pvz., "Patvirtinimas – "SharePoint 2010") į sąrašą arba biblioteką.</span><span class="sxs-lookup"><span data-stu-id="ae517-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="ae517-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="ae517-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="ae517-105">Atidarykite svetainių rinkinio šakninę svetainę naudodami "SharePoint Designer 2013".</span><span class="sxs-lookup"><span data-stu-id="ae517-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="ae517-106">Dalyje **Svetainės objektai**pasirinkite Darbo **eigos**.</span><span class="sxs-lookup"><span data-stu-id="ae517-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="ae517-107">Juostelės **Darbo eigos** sekcijoje **Naujas** pasirinkite **Daugkartinio naudojimo darbo eiga**.</span><span class="sxs-lookup"><span data-stu-id="ae517-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="ae517-108">Formoje **Kurti pakartotinai naudoti darbo eigą** įveskite pavadinimą \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="ae517-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="ae517-109">**Platformos tipo**spustelėkite **SharePoint 2010 darbo eiga**, tada spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="ae517-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="ae517-110">Juostelės **Darbo eiga** sekcijoje **Įrašyti** pasirinkite **Publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="ae517-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="ae517-111">Juostelės **Darbo** **eiga** sekcijoje Tvarkyti pasirinkite **Publikuoti visame pasaulyje**.</span><span class="sxs-lookup"><span data-stu-id="ae517-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="ae517-112">Pasirodžiusiame patvirtinimo dialogo lange pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="ae517-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="ae517-113">Žiniatinklio naršyklėje raskite svetainių rinkinio šakninę svetainę ir pasiekite **Svetainės parametrų** \> **svetainių rinkinio funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="ae517-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="ae517-114">Perjunkite **darbo eigų** funkciją:</span><span class="sxs-lookup"><span data-stu-id="ae517-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="ae517-115">· Jei priemonė *suaktyvinta* , spustelėkite **Išjungti,** tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="ae517-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="ae517-116">· Jei funkcija *išjungta* , spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="ae517-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="ae517-117">Daugiau informacijos rasite šiame [straipsnyje](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ae517-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

