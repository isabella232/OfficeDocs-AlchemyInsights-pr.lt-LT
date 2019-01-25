---
title: Negalima įtraukti numatytąjį 2010 patvirtinimo darbo eiga
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480127"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="879c9-102">Negalima įtraukti numatytąjį 2010 patvirtinimo darbo eiga</span><span class="sxs-lookup"><span data-stu-id="879c9-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="879c9-103">Microsoft SharePoint svetainių rinkinio, visame pasaulyje daugkartinio naudojimo darbo eigą (pvz., "patvirtinimo – SharePoint 2010") negalima įtraukti į sąrašą ar biblioteką.</span><span class="sxs-lookup"><span data-stu-id="879c9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="879c9-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="879c9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="879c9-105">Atidarykite šaknų svetainėje svetainių rinkinio SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="879c9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="879c9-106">Pagal **Svetainėje objektų**, pasirinkite **darbo eigos**.</span><span class="sxs-lookup"><span data-stu-id="879c9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="879c9-107">**Darbo eigos** juosta **Naujoji** dalyje pasirinkite **Darbo eigos pakartotinai**.</span><span class="sxs-lookup"><span data-stu-id="879c9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="879c9-p101">**Sukurti daugkartinio naudojimo darbo eigos** formoje, įvardykite \* \*\*Repair2010\*\*\*. **Platformos tipas**, pasirinkite **SharePoint 2010 darbo eigos**, ir pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="879c9-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="879c9-110">**Įrašyti** **darbo eigos** juosta dalyje pasirinkite **publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="879c9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="879c9-p102">**Darbo eigos** juosta sekcijoje **tvarkyti** pasirinkite **Visame pasaulyje skelbia**. Patvirtinimo dialogo lange, kuris pasirodo, pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="879c9-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="879c9-p103">Naudodami žiniatinklio naršyklę, raskite šakninio svetainės svetainių rinkinio ir tada naudotis **Svetainės parametrai** \> **Svetainės rinkinio funkcijos**. Tada perjungti **darbo eigos** funkcija:</span><span class="sxs-lookup"><span data-stu-id="879c9-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="879c9-115">· Jei ši funkcija yra *aktyvuota* , spustelėkite **išjungti,** ir tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="879c9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="879c9-116">· Jei ši funkcija yra *Deactivated* , spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="879c9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="879c9-117">Norėdami gauti daugiau informacijos prašome kreiptis į šį [straipsnį](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="879c9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

