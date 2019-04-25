---
title: Svetainę ar sąrašą įrašyti kaip šabloną
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243525"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="83b70-102">Svetainę ar sąrašą įrašyti kaip šabloną</span><span class="sxs-lookup"><span data-stu-id="83b70-102">Save site or list as a template</span></span>

<span data-ttu-id="83b70-103">SharePoint svetainės šablonuose yra iš anksto įdėtus apibrėžtis, skirta apie konkretaus verslo poreikiams.</span><span class="sxs-lookup"><span data-stu-id="83b70-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="83b70-104">Norėdami gauti daugiau informacijos, peržiūrėkite [naudojant šablonus kurti įvairių rūšių "SharePoint" svetaines](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="83b70-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="83b70-105">Čia yra kai kurių bendrų klausimų/sprendimų dėl taupymo svetainės ar sąrašo kaip šabloną SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="83b70-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="83b70-106">**Išsaugoti sąraše tinklapis nėra prieinama arba jis yra šabloną mygtuką**.</span><span class="sxs-lookup"><span data-stu-id="83b70-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="83b70-107">Administratoriai reikia leisti Custom scenarijų įgalinti šablono savybės.</span><span class="sxs-lookup"><span data-stu-id="83b70-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="83b70-108">Išsamius veiksmus, pavyzdžiai ir svarstymus žr [leisti arba neleisti pasirinktinį scenarijų](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="83b70-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="83b70-109">Įrašyti svetainę kaip šabloną komandą nepalaikomas ir gali kilti problemų dėl svetainių, kurios naudoja SharePoint serverio publikavimo infrastruktūra.</span><span class="sxs-lookup"><span data-stu-id="83b70-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="83b70-110">**Svetainės šablonas negali būti sukurta ar veikia netinkamai**</span><span class="sxs-lookup"><span data-stu-id="83b70-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="83b70-111">Šablonas gali trūkti [funkciją](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ir nebus aktyvinta.</span><span class="sxs-lookup"><span data-stu-id="83b70-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="83b70-112">Jei funkcija nėra įjungti į dabartinio svetainių rinkinio, svetainės šabloną negalite sukurti svetainę.</span><span class="sxs-lookup"><span data-stu-id="83b70-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="83b70-113">Patikrinkite, jei jokių sąrašų arba bibliotekų viršija [Sąrašo rodinio slenkstį limitas](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) yra 5000 elementų, kaip tai gali blokuoti svetainės šabloną sukurti.</span><span class="sxs-lookup"><span data-stu-id="83b70-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="83b70-114">Svetainės gali naudoti per daug išteklių ir todėl svetainės šabloną viršija 50 megabaitų (MB) limitą.</span><span class="sxs-lookup"><span data-stu-id="83b70-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="83b70-115">Yra problemų Rodyti duomenis iš sąrašo, kuris naudoja peržvalgos stulpelio.</span><span class="sxs-lookup"><span data-stu-id="83b70-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="83b70-116">Daugiau informacijos ieškokite [sąrašo šabloną sukurtas nerodo duomenų teisingą peržvalgos sąrašo SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="83b70-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="83b70-117">Daugiau informacijos apie bendras problemas ir sprendimus, prašome nuoroda, [kurti ir naudoti svetainės šablonai](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="83b70-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

