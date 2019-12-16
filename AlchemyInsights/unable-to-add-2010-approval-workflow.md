---
title: Neįmanoma pridėti 2010 patvirtinimo darbo eigos
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049561"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="eaf86-102">Neįmanoma pridėti 2010 patvirtinimo darbo eigos</span><span class="sxs-lookup"><span data-stu-id="eaf86-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="eaf86-103">Microsoft SharePoint svetainių rinkinyje negalite įtraukti visuotinai pakartotinai naudojamos darbo eigos (pvz., "patvirtinimas-SharePoint 2010") į sąrašą arba biblioteką.</span><span class="sxs-lookup"><span data-stu-id="eaf86-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="eaf86-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="eaf86-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="eaf86-105">SharePoint Designer 2013 atidarykite svetainių rinkinio šakninę svetainę.</span><span class="sxs-lookup"><span data-stu-id="eaf86-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="eaf86-106">Dalyje **svetainės objektai**pasirinkite **darbo eigos**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="eaf86-107">**Darbo eigos** juostelės **naujoje** sekcijoje pasirinkite **daugkartinio naudojimo darbo eiga**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="eaf86-108">Formoje **kurti pakartotinai naudojamą darbo eigą** įveskite pavadinimą \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="eaf86-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="eaf86-109">**Platformos tipas**, spustelėkite **SharePoint 2010 darbo eiga**, ir tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="eaf86-110">**Darbo eigos** juostelės sekcijoje **įrašyti** pasirinkite **publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="eaf86-111">**Darbo eigos** juostelės sekcijoje **tvarkyti** pasirinkite **publikuoti visuotinai**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="eaf86-112">Pasirodžiusiame patvirtinimo dialogo lange pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="eaf86-113">Žiniatinklio naršyklėje raskite šakninę svetainių rinkinio svetainę ir pasiekite svetainės **parametrų** \> **svetainių rinkinio funkcijas**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="eaf86-114">Perjunkite **darbo eigų** funkciją:</span><span class="sxs-lookup"><span data-stu-id="eaf86-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="eaf86-115">· Jei funkcija *suaktyvinta* , spustelėkite **išjungti,** tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="eaf86-116">· Jei funkcija *išjungiama* , spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="eaf86-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="eaf86-117">Daugiau informacijos rasite šiame [straipsnyje](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="eaf86-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

