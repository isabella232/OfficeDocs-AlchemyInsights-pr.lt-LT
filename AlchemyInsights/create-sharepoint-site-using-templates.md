---
title: Svetainės kūrimas SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052477"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="f9f62-102">"SharePoint" svetainių kūrimas naudojant šablonus</span><span class="sxs-lookup"><span data-stu-id="f9f62-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="f9f62-103">SharePoint svetainių šablonai yra iš anksto sukurti apibrėžimai, skirti tam tikram verslo poreikiui.</span><span class="sxs-lookup"><span data-stu-id="f9f62-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="f9f62-104">Daugiau informacijos rasite [šablonų naudojimas skirtingoms "SharePoint" svetainių rūšims kurti](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="f9f62-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="f9f62-105">Čia pateikiamos kelios Dažnos problemos/sprendimai dėl svetainės ar sąrašo įrašymo kaip "SharePoint Online" šablono.</span><span class="sxs-lookup"><span data-stu-id="f9f62-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="f9f62-106">**Mygtukas įrašyti svetainės/sąrašo šabloną yra neprieinamas arba jo nėra**</span><span class="sxs-lookup"><span data-stu-id="f9f62-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="f9f62-107">Administratoriams reikės leisti pasirinktinį scenarijų, kad įgalintumėte šablono funkcijas.</span><span class="sxs-lookup"><span data-stu-id="f9f62-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="f9f62-108">Išsamius veiksmus, pavyzdžius ir svarstymus žr.</span><span class="sxs-lookup"><span data-stu-id="f9f62-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="f9f62-109">Leisti arba neleisti pasirinktinio scenarijaus</span><span class="sxs-lookup"><span data-stu-id="f9f62-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="f9f62-110">Komanda įrašyti svetainę kaip šabloną nepalaikoma ir gali sukelti problemų svetainėse, kurios naudoja SharePoint serverio publikavimo infrastruktūrą.</span><span class="sxs-lookup"><span data-stu-id="f9f62-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="f9f62-111">**Neįmanoma sukurti svetainės šablono arba tinkamai neveikti**</span><span class="sxs-lookup"><span data-stu-id="f9f62-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="f9f62-112">Šablone gali trūkti [funkcijos](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ir jos neaktyvinti.</span><span class="sxs-lookup"><span data-stu-id="f9f62-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="f9f62-113">Jei šios funkcijos negalima aktyvinti dabartiniame svetainių rinkinyje, svetainės šablono negalite naudoti kurdami svetainę.</span><span class="sxs-lookup"><span data-stu-id="f9f62-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="f9f62-114">Patikrinkite, ar sąrašai ir bibliotekos viršija 5000 elementų [sąrašo rodinio ribinę vertę](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , nes tai gali blokuoti svetainės šablono kūrimą.</span><span class="sxs-lookup"><span data-stu-id="f9f62-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="f9f62-115">Svetainė gali naudoti per daug išteklių, todėl svetainės šablonas viršija 50 MB limitą.</span><span class="sxs-lookup"><span data-stu-id="f9f62-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="f9f62-116">Yra problemų rodant duomenis iš sąrašo, kuris naudoja peržvalgos stulpelį.</span><span class="sxs-lookup"><span data-stu-id="f9f62-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="f9f62-117">Daugiau informacijos ieškokite [šablono sugeneruotas sąraše nerodo duomenis iš tinkamą peržvalgos sąrašą SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="f9f62-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="f9f62-118">Norėdami gauti išsamesnės informacijos apie bendrąsias problemas ir sprendimus, patikrinkite [kurti ir naudoti svetainės šablonus](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="f9f62-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



