---
title: Darbo eiga nepradedama
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794775"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="f3179-102">Darbo eiga nepradedama</span><span class="sxs-lookup"><span data-stu-id="f3179-102">Workflow is not starting</span></span>

- <span data-ttu-id="f3179-103">"SharePoint 2010" ir "SharePoint 2013" darbo eigos nepaleidžiamos.</span><span class="sxs-lookup"><span data-stu-id="f3179-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="f3179-104">Jei darbo eiga nepradedama, gali būti laikina aptarnavimo problema, kai vartotojai gali susidurti su pertrūkiais dėl darbo eigos eigos.</span><span class="sxs-lookup"><span data-stu-id="f3179-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="f3179-105">Patikrinkite [tarnybos sveikatos ataskaitų sritį](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) ir Sužinokite, ar jūsų organizacija turi įtakos.</span><span class="sxs-lookup"><span data-stu-id="f3179-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="f3179-106">Jei praėjo daugiau nei 24 valandos po to, kai pirmą kartą matėte šią problemą, prisijunkite prie palaikymo bilieto.</span><span class="sxs-lookup"><span data-stu-id="f3179-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f3179-107">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="f3179-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f3179-108">Pateikite mums bent 24 valandas, kad užbaigtumėte sprendimą.</span><span class="sxs-lookup"><span data-stu-id="f3179-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="f3179-109">"SharePoint 2010" darbo eigos vėluoja pradėti.</span><span class="sxs-lookup"><span data-stu-id="f3179-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="f3179-110">Taip nutinka, jei darbo eiga suaktyvinama dideliais paketais.</span><span class="sxs-lookup"><span data-stu-id="f3179-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="f3179-111">(pvz., kai keli elementai įtraukiami vienu metu).</span><span class="sxs-lookup"><span data-stu-id="f3179-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="f3179-112">Darbo eigos nėra sukurtos veikti realiuoju laiku, todėl vėlavimas yra dizaino elgesys.</span><span class="sxs-lookup"><span data-stu-id="f3179-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="f3179-113">Jei darbo eiga yra sudėtinga Išplėstinė objekto aprašų kalba (XMOL), Kompiliacija gali būti lėta.</span><span class="sxs-lookup"><span data-stu-id="f3179-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="f3179-114">Pažymėkite [šį](https://support.microsoft.com//kb/3043697) straipsnį.</span><span class="sxs-lookup"><span data-stu-id="f3179-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="f3179-115">Turėtumėte supaprastinti darbo eigą arba perdaryti ją naudodami "Microsoft SharePoint 2013" darbo eigos platformos tipą.</span><span class="sxs-lookup"><span data-stu-id="f3179-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="f3179-116">Jei jūsų darbo eigos retrospektyva išaugo daug, galbūt norėsite išvalyti elementus arba kurti naują retrospektyvos sąrašą.</span><span class="sxs-lookup"><span data-stu-id="f3179-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="f3179-117">Daugiau informacijos: [darbo eigos retrospektyvos](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/) šalinimas</span><span class="sxs-lookup"><span data-stu-id="f3179-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="f3179-118">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="f3179-118">Related topics</span></span>
<span data-ttu-id="f3179-119">Norite išbandyti "Microsoft Flow" "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="f3179-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="f3179-120">Kurti srautą</span><span class="sxs-lookup"><span data-stu-id="f3179-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f3179-121">"SharePoint" ir srautas</span><span class="sxs-lookup"><span data-stu-id="f3179-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


