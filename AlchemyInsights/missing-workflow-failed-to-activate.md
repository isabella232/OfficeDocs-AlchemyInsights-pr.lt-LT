---
title: Trūksta darbo eigos nepavyko aktyvinti
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917576"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9bdda-102">Trūksta darbo eigos nepavyko aktyvinti</span><span class="sxs-lookup"><span data-stu-id="9bdda-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9bdda-103">Microsoft SharePoint svetainių rinkinio, visame pasaulyje daugkartinio naudojimo darbo eigą (pvz., "patvirtinimo – SharePoint 2010") negalima įtraukti į sąrašą ar biblioteką.</span><span class="sxs-lookup"><span data-stu-id="9bdda-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9bdda-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="9bdda-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9bdda-105">Atidarykite šaknų svetainėje svetainių rinkinio SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9bdda-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9bdda-106">Pagal **Svetainėje objektų**, pasirinkite **darbo eigos**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9bdda-107">**Darbo eigos** juosta **Naujoji** dalyje pasirinkite **Darbo eigos pakartotinai**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9bdda-p101">**Sukurti daugkartinio naudojimo darbo eigos** formoje, įvardykite \*\* *Repair2010* \*\*. **Platformos tipas**, spustelėkite **SharePoint 2010 darbo eigos**, ir tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9bdda-110">**Įrašyti** **darbo eigos** juosta dalyje pasirinkite **publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9bdda-p102">**Darbo eigos** juosta sekcijoje **tvarkyti** pasirinkite **Visame pasaulyje skelbia**. Patvirtinimo dialogo lange, kuris pasirodo, pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9bdda-p103">Naudodami žiniatinklio naršyklę, raskite šakninio svetainės svetainių rinkinio ir tada naudotis **Svetainės parametrai** \> **Svetainės rinkinio funkcijos**. Tada perjungti **darbo eigos** funkcija:</span><span class="sxs-lookup"><span data-stu-id="9bdda-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9bdda-115">· Jei ši funkcija yra *aktyvuota* , spustelėkite **išjungti,** ir tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9bdda-116">· Jei ši funkcija yra *Deactivated* , spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="9bdda-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9bdda-117">Norėdami gauti daugiau informacijos prašome kreiptis į šį [straipsnį](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9bdda-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

