---
title: Nepavyko suaktyvinti trūkstamos darbo eigos
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667094"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8cb4e-102">Nepavyko suaktyvinti trūkstamos darbo eigos</span><span class="sxs-lookup"><span data-stu-id="8cb4e-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8cb4e-103">"Microsoft SharePoint" svetainių rinkinyje negalite įtraukti globaliai pakartotinai naudojamos darbo eigos (pvz., "patvirtinimas –" SharePoint 2010 ") į sąrašą arba biblioteką.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8cb4e-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8cb4e-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8cb4e-105">Atidarykite svetainių rinkinio svetainę "SharePoint Designer 2013".</span><span class="sxs-lookup"><span data-stu-id="8cb4e-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8cb4e-106">Dalyje **svetainės objektai**pasirinkite **darbo eigos**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8cb4e-107">Juostelėje esančioje **naujoje** **darbo** eigos sekcijoje pasirinkite pakartotinai naudojama **darbo eiga**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8cb4e-108">Formoje **kurti pakartotinai naudojamą darbo eigą** , parašykite pavadinimą \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8cb4e-109">Jei turite **platformos tipą**, spustelėkite " **SharePoint 2010" darbo eiga**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8cb4e-110">**Darbo eigos** juostelės sekcijoje **įrašyti** pasirinkite **publikuoti**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8cb4e-111">**Darbo eigos** juostelės sekcijoje **tvarkyti** pasirinkite **publikuoti visuotinai**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8cb4e-112">Rodomame patvirtinimo dialogo lange pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8cb4e-113">Žiniatinklio naršyklėje raskite svetainių rinkinio svetainę, tada pasiekite svetainės **parametrų** \> **svetainių rinkinio funkcijas**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8cb4e-114">Tada perjunkite **darbo eigų** funkciją:</span><span class="sxs-lookup"><span data-stu-id="8cb4e-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8cb4e-115">· Jei funkcija  *suaktyvinta*  , spustelėkite **išjungti,** tada spustelėkite **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8cb4e-116">· Jei funkcija  *išjungta, spustelėkite* **Aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="8cb4e-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8cb4e-117">Daugiau informacijos ieškokite šiame [straipsnyje](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8cb4e-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

