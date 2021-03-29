---
title: Darbo eiga nepaleidžianti
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403751"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="05dc3-102">Darbo eiga nepaleidžianti</span><span class="sxs-lookup"><span data-stu-id="05dc3-102">Workflow is not starting</span></span>

- <span data-ttu-id="05dc3-103">"SharePoint 2010" ir "SharePoint 2013" darbo eigos nepaleidžiant.</span><span class="sxs-lookup"><span data-stu-id="05dc3-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="05dc3-104">Jei jūsų darbo eiga nepaleidžianti, gali būti laikina tarnybos problema, dėl kurios vartotojai gali patirti su pertrūkiais uždelstą darbo eigos eigą.</span><span class="sxs-lookup"><span data-stu-id="05dc3-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="05dc3-105">Patikrinkite tarnybos [sveikatos ataskaitų sritį,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) kad pamatytumėte, ar paveikta jūsų organizacija.</span><span class="sxs-lookup"><span data-stu-id="05dc3-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="05dc3-106">Jei praėjo daugiau nei 24 valandos nuo tada, kai pirmą kartą matėte šią problemą, prisijunkite prie palaikymo kvito.</span><span class="sxs-lookup"><span data-stu-id="05dc3-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="05dc3-107">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="05dc3-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="05dc3-108">Pateikite mums bent 24 valandas, kad užbaigtų sprendimą.</span><span class="sxs-lookup"><span data-stu-id="05dc3-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="05dc3-109">"SharePoint 2010" darbo eigos vėluoja pradėti.</span><span class="sxs-lookup"><span data-stu-id="05dc3-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="05dc3-110">Taip nutinka, jei darbo eiga paleidžiama dideliuose paketuose.</span><span class="sxs-lookup"><span data-stu-id="05dc3-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="05dc3-111">(pvz., kai vienu metu įtraukiami keli elementai).</span><span class="sxs-lookup"><span data-stu-id="05dc3-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="05dc3-112">Darbo eigos nėra skirtos veikti realiuoju laiku, todėl delsa yra dizaino veikimas.</span><span class="sxs-lookup"><span data-stu-id="05dc3-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="05dc3-113">Jei darbo eiga yra sudėtinga sudėtingesnė objekto žymėjimo kalba (XMOL), kompiliavimas gali būti lėtas.</span><span class="sxs-lookup"><span data-stu-id="05dc3-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="05dc3-114">Peržiūrėkite [šį](https://support.microsoft.com//kb/3043697) straipsnį.</span><span class="sxs-lookup"><span data-stu-id="05dc3-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="05dc3-115">Turėtumėte supaprastinti darbo eigą arba perkurti ją naudodami "Microsoft SharePoint 2013 Workflow" platformos tipą.</span><span class="sxs-lookup"><span data-stu-id="05dc3-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="05dc3-116">Jei jūsų darbo eigos retrospektyva išaugo, galbūt norėsite išvalyti elementus arba sukurti naują retrospektyvos sąrašą.</span><span class="sxs-lookup"><span data-stu-id="05dc3-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="05dc3-117">Daugiau informacijos: [Darbo eigos retrospektyvos valymas](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="05dc3-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="05dc3-118">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="05dc3-118">Related topics</span></span>
<span data-ttu-id="05dc3-119">Norite išbandyti "Microsoft Flow" programoje "SharePoint Online"?</span><span class="sxs-lookup"><span data-stu-id="05dc3-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="05dc3-120">Srauto kūrimas</span><span class="sxs-lookup"><span data-stu-id="05dc3-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="05dc3-121">"SharePoint" ir "Flow"</span><span class="sxs-lookup"><span data-stu-id="05dc3-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
