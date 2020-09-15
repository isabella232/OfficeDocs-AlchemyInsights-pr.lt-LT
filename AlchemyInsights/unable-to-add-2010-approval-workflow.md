---
title: Nepavyksta įtraukti 2010 patvirtinimo darbo eigos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699743"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="448e5-102">Nepavyksta įtraukti 2010 patvirtinimo darbo eigos</span><span class="sxs-lookup"><span data-stu-id="448e5-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="448e5-103">"Microsoft SharePoint" svetainių rinkinyje negalite įtraukti globaliai pakartotinai naudojamos darbo eigos (pvz., "patvirtinimas –" SharePoint 2010 ") į sąrašą arba biblioteką.</span><span class="sxs-lookup"><span data-stu-id="448e5-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="448e5-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="448e5-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="448e5-105">Atidarykite svetainių rinkinio svetainę "SharePoint Designer 2013".</span><span class="sxs-lookup"><span data-stu-id="448e5-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="448e5-106">Dalyje **svetainės objektai**pasirinkite **darbo eigos**.</span><span class="sxs-lookup"><span data-stu-id="448e5-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="448e5-107">Juostelėje esančioje **naujoje** **darbo** eigos sekcijoje pasirinkite pakartotinai naudojama **darbo eiga**.</span><span class="sxs-lookup"><span data-stu-id="448e5-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="448e5-108">Formoje **kurti pakartotinai naudojamą darbo eigą** , parašykite pavadinimą \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="448e5-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="448e5-109">Jei turite **platformos tipą**, spustelėkite " **SharePoint 2010" darbo eiga**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="448e5-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="448e5-110">**Darbo eigos** juostelės sekcijoje **įrašyti** pasirinkite **publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="448e5-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="448e5-111">**Darbo eigos** juostelės sekcijoje **tvarkyti** pasirinkite **publikuoti visuotinai**.</span><span class="sxs-lookup"><span data-stu-id="448e5-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="448e5-112">Rodomame patvirtinimo dialogo lange pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="448e5-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="448e5-113">Žiniatinklio naršyklėje raskite svetainių rinkinio svetainę, tada pasiekite svetainės **parametrų** \> **svetainių rinkinio funkcijas**.</span><span class="sxs-lookup"><span data-stu-id="448e5-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="448e5-114">Perjungti **darbo eigų** funkciją:</span><span class="sxs-lookup"><span data-stu-id="448e5-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="448e5-115">· Jei funkcija  *suaktyvinta*  , spustelėkite **išjungti,** tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="448e5-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="448e5-116">· Jei funkcija  *išjungta, spustelėkite* **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="448e5-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="448e5-117">Daugiau informacijos ieškokite šiame [straipsnyje](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="448e5-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

