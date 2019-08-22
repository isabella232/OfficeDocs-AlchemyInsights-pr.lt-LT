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
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543933"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="1b7f4-102">Trūksta darbo eigos nepavyko aktyvinti</span><span class="sxs-lookup"><span data-stu-id="1b7f4-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="1b7f4-103">Microsoft SharePoint svetainių rinkinio, visame pasaulyje daugkartinio naudojimo darbo eigą (pvz., "patvirtinimo – SharePoint 2010") negalima įtraukti į sąrašą ar biblioteką.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="1b7f4-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="1b7f4-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="1b7f4-105">Atidarykite šaknų svetainėje svetainių rinkinio SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="1b7f4-106">Pagal **Svetainėje objektų**, pasirinkite **darbo eigos**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="1b7f4-107">**Darbo eigos** juosta **Naujoji** dalyje pasirinkite **Darbo eigos pakartotinai**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="1b7f4-108">**Sukurti daugkartinio naudojimo darbo eigos** formoje, įvardykite \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="1b7f4-109">**Platformos tipas**, spustelėkite **SharePoint 2010 darbo eigos**, ir tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="1b7f4-110">**Įrašyti** **darbo eigos** juosta dalyje pasirinkite **publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="1b7f4-111">**Darbo eigos** juosta sekcijoje **tvarkyti** pasirinkite **Visame pasaulyje skelbia**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="1b7f4-112">Patvirtinimo dialogo lange, kuris pasirodo, pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="1b7f4-113">Naudodami žiniatinklio naršyklę, raskite šakninio svetainės svetainių rinkinio ir tada naudotis **Svetainės parametrai** \> **Svetainės rinkinio funkcijos**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="1b7f4-114">Tada perjungti **darbo eigos** funkcija:</span><span class="sxs-lookup"><span data-stu-id="1b7f4-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="1b7f4-115">· Jei ši funkcija yra *aktyvuota* , spustelėkite **išjungti,** ir tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="1b7f4-116">· Jei ši funkcija yra *Deactivated* , spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="1b7f4-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="1b7f4-117">Norėdami gauti daugiau informacijos prašome kreiptis į šį [straipsnį](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="1b7f4-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

