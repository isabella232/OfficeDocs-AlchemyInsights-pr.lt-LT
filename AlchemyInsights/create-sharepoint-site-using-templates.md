---
title: Sukurti svetainę, SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199281"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="e7e0e-102">Kurti SharePoint svetaines naudojant šablonus</span><span class="sxs-lookup"><span data-stu-id="e7e0e-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="e7e0e-103">SharePoint svetainės šablonuose yra iš anksto įdėtus apibrėžtis, skirta apie konkretaus verslo poreikiams.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="e7e0e-104">Norėdami gauti daugiau informacijos, peržiūrėkite [naudojant šablonus kurti įvairių rūšių "SharePoint" svetaines](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="e7e0e-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="e7e0e-105">Čia yra kai kurių bendrų klausimų/sprendimų dėl taupymo svetainės ar sąrašo kaip šabloną Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="e7e0e-106">**Išsaugoti sąraše tinklapis šabloną mygtuką nėra ar ji nėra**</span><span class="sxs-lookup"><span data-stu-id="e7e0e-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="e7e0e-107">Administratoriai reikia leisti Custom scenarijų įgalinti šablono savybės.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="e7e0e-108">Išsamius veiksmus, rasite pavyzdžių ir aplinkybes</span><span class="sxs-lookup"><span data-stu-id="e7e0e-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="e7e0e-109">Leisti arba neleisti pasirinktinį scenarijų</span><span class="sxs-lookup"><span data-stu-id="e7e0e-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="e7e0e-110">Įrašyti svetainę kaip šabloną komandą nepalaikomas ir gali kilti problemų dėl svetainių, kurios naudoja SharePoint serverio publikavimo infrastruktūra.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="e7e0e-111">**Svetainės šablonas negali būti sukurta ar veikia netinkamai**</span><span class="sxs-lookup"><span data-stu-id="e7e0e-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="e7e0e-112">Šablonas gali trūkti [funkciją](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ir nebus aktyvinta.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="e7e0e-113">Jei funkcija nėra įjungti į dabartinio svetainių rinkinio, svetainės šabloną negalite sukurti svetainę.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="e7e0e-114">Patikrinkite, jei jokių sąrašų arba bibliotekų viršija [Sąrašo rodinio slenkstį limitas](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) yra 5000 elementų, kaip tai gali blokuoti svetainės šabloną sukurti.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="e7e0e-115">Svetainės gali naudoti per daug išteklių, ir todėl svetainės šabloną viršija 50 MB limito.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="e7e0e-116">Yra problemų Rodyti duomenis iš sąrašo, kuris naudoja peržvalgos stulpelio.</span><span class="sxs-lookup"><span data-stu-id="e7e0e-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="e7e0e-117">Daugiau informacijos ieškokite [sąrašo šabloną sukurtas nerodo duomenų teisingą peržvalgos sąrašo SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="e7e0e-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="e7e0e-118">Išsamesnė informacija apie bendrosios problemos ir jų sprendimai, prašome patikrinti [svetainių šablonų kūrimas ir naudojimas](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="e7e0e-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



