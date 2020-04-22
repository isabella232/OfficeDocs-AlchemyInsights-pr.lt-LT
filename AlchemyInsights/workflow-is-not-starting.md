---
title: Darbo eiga nepradedama
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766105"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="2a2d6-102">Darbo eiga nepradedama</span><span class="sxs-lookup"><span data-stu-id="2a2d6-102">Workflow is not starting</span></span>

- <span data-ttu-id="2a2d6-103">Nepaleidžiama "SharePoint 2010" ir "SharePoint 2013" darbo eigos.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="2a2d6-104">Jei jūsų darbo eiga neprasideda, gali būti laikina tarnybos problema, kai vartotojai gali susidurti su pasikartojančiais delsa darbo eigos eiga.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="2a2d6-105">Patikrinkite [tarnybos sveikatos ataskaitų sritį,](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) kad sužinotumėte, ar jūsų organizacijai daromas poveikis.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="2a2d6-106">Jei praėjo daugiau nei 24 valandos nuo to laiko, kai pirmą kartą matėte šią problemą, prisijunkite palaikymo bilietą.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="2a2d6-107">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2a2d6-108">Prašome duoti mums ne mažiau kaip 24 valandas užbaigti sprendimą.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="2a2d6-109">"SharePoint 2010" darbo eigos vėluoja paleisti.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="2a2d6-110">Taip nutinka, jei darbo eiga paleidžiama dideliais paketais.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="2a2d6-111">(pvz., kai vienu metu pridedami keli elementai).</span><span class="sxs-lookup"><span data-stu-id="2a2d6-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="2a2d6-112">Darbo eigos nėra skirtos veikti realiuoju laiku, todėl delsa yra pagal dizainą.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="2a2d6-113">Jei darbo eiga yra sudėtinga išplėstinė objekto aprašų kalba (XMOL), kompiliavimas gali būti lėtas.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="2a2d6-114">Patikrinkite [šį](https://support.microsoft.com//kb/3043697) straipsnį.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="2a2d6-115">Turėtumėte supaprastinti darbo eigą arba pertvarkyti ją naudodami "Microsoft SharePoint 2013" darbo eigos platformos tipą.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="2a2d6-116">Jei jūsų darbo eigos retrospektyva išaugo didelis, galbūt norėsite išvalyti elementus arba sukurti naują retrospektyvos sąrašą.</span><span class="sxs-lookup"><span data-stu-id="2a2d6-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="2a2d6-117">Daugiau informacijos : [Išvalyti darbo eigos retrospektyvą](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="2a2d6-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="2a2d6-118">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="2a2d6-118">Related topics</span></span>
<span data-ttu-id="2a2d6-119">Norite išbandyti "Microsoft Flow" "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="2a2d6-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2a2d6-120">Kurti srautą</span><span class="sxs-lookup"><span data-stu-id="2a2d6-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2a2d6-121">"SharePoint" ir srautas</span><span class="sxs-lookup"><span data-stu-id="2a2d6-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


