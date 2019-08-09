---
title: Darbo eigos nepasileidžia
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270788"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="9d58c-102">Darbo eigos nepasileidžia</span><span class="sxs-lookup"><span data-stu-id="9d58c-102">Workflow is not starting</span></span>

- <span data-ttu-id="9d58c-103">SharePoint 2010 ir SharePoint 2013 darbo eigos nepasileidžia.</span><span class="sxs-lookup"><span data-stu-id="9d58c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="9d58c-104">Jei jūsų darbo eigos paleisti nepavyksta, gali būti laikinai tarnybos problema tais atvejais, kai vartotojai gali patirti vėlinimų su darbo eigos pažangą.</span><span class="sxs-lookup"><span data-stu-id="9d58c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="9d58c-105">Patikrinkite [Tarnybų sveikatos stebėjimo skydas](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) Norėdami pamatyti, jei jūsų organizacija smūgiuoja.</span><span class="sxs-lookup"><span data-stu-id="9d58c-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="9d58c-106">Jei daugiau nei 24 valandų praėjo nuo pirmą kartą pamačiau šią problemą, prašome prisijungti support ticket.</span><span class="sxs-lookup"><span data-stu-id="9d58c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9d58c-107">Daugeliu atvejų, mes jau dirbame išeitį.</span><span class="sxs-lookup"><span data-stu-id="9d58c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9d58c-108">Nurodykite bent 24 valandas atlikti sprendimą.</span><span class="sxs-lookup"><span data-stu-id="9d58c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="9d58c-109">SharePoint 2010 darbo eigos atidėtas pradžios ekrane.</span><span class="sxs-lookup"><span data-stu-id="9d58c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="9d58c-110">Tai įvyksta, jei darbo eigos yra užfiksuojamas didelėmis partijomis.</span><span class="sxs-lookup"><span data-stu-id="9d58c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="9d58c-111">(pvz., kai keli elementai įtraukiami vienu metu).</span><span class="sxs-lookup"><span data-stu-id="9d58c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="9d58c-112">Darbo eigos skirtos ne paleisti realiu laiku, todėl vėluoja projektuojant elgesį.</span><span class="sxs-lookup"><span data-stu-id="9d58c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="9d58c-113">Jei darbo eigos yra sudėtinga Išplėstinė objekto žymėjimo kalba (XMOL), rengimo gali sulėtėti.</span><span class="sxs-lookup"><span data-stu-id="9d58c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="9d58c-114">Patikrinkite, ar [šiame](https://support.microsoft.com/en-us/kb/3043697) straipsnyje.</span><span class="sxs-lookup"><span data-stu-id="9d58c-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="9d58c-115">Reikėtų supaprastinti darbo eigą ar pertvarkyti naudodami Microsoft SharePoint 2013 darbo eigos platformos tipo.</span><span class="sxs-lookup"><span data-stu-id="9d58c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="9d58c-116">Jei jūsų darbo eigos retrospektyvos išaugo didelis, galite išvalyti elementus arba kurti naują istorijos sąrašą.</span><span class="sxs-lookup"><span data-stu-id="9d58c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="9d58c-117">Daugiau informacijos: [Šalinti darbo eigos retrospektyvos](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="9d58c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="9d58c-118">Susijusios temos</span><span class="sxs-lookup"><span data-stu-id="9d58c-118">Related topics</span></span>
<span data-ttu-id="9d58c-119">Norite išbandyti Microsoft Flow SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="9d58c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9d58c-120">Sukurti srauto</span><span class="sxs-lookup"><span data-stu-id="9d58c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9d58c-121">SharePoint ir srauto</span><span class="sxs-lookup"><span data-stu-id="9d58c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


