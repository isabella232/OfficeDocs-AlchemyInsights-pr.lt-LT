---
title: Svetainės arba sąrašo įrašymas kaip šablono
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727539"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="4631f-102">Svetainės arba sąrašo įrašymas kaip šablono</span><span class="sxs-lookup"><span data-stu-id="4631f-102">Save site or list as a template</span></span>

<span data-ttu-id="4631f-103">"SharePoint" svetainės šablonai yra iš anksto sukurtos apibrėžtys, skirtos konkrečiam verslo poreikiui.</span><span class="sxs-lookup"><span data-stu-id="4631f-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="4631f-104">Daugiau informacijos rasite [šablonų naudojimas kuriant skirtingų](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)tipų "SharePoint" svetaines.</span><span class="sxs-lookup"><span data-stu-id="4631f-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="4631f-105">Štai keletas dažniausių problemų/sprendimų dėl svetainės arba sąrašo įrašymo kaip "SharePoint Online" šablono.</span><span class="sxs-lookup"><span data-stu-id="4631f-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="4631f-106">**Mygtukas įrašyti svetainės/sąrašo šablono nėra arba jo**nėra.</span><span class="sxs-lookup"><span data-stu-id="4631f-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="4631f-107">Administratoriams reikės leisti pasirinktiniam scenarijui įgalinti šablono funkcijas.</span><span class="sxs-lookup"><span data-stu-id="4631f-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="4631f-108">Išsamių veiksmų, pavyzdžių ir svarstymų ieškokite [pasirinktinio scenarijaus leidimas arba neleidimas](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="4631f-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="4631f-109">Komanda įrašyti svetainę kaip šabloną nepalaikoma, todėl gali kilti problemų svetainėse, naudojančioms "SharePoint Server" publikavimo infrastruktūrą.</span><span class="sxs-lookup"><span data-stu-id="4631f-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="4631f-110">**Negalima sukurti svetainės šablono arba jis veikia netinkamai**</span><span class="sxs-lookup"><span data-stu-id="4631f-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="4631f-111">Šablonui gali trūkti [funkcijos](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ir jis nebus suaktyvintas.</span><span class="sxs-lookup"><span data-stu-id="4631f-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="4631f-112">Jei šios funkcijos negalima aktyvinti dabartiniame svetainių rinkinyje, svetainės šablono negalite naudoti svetainei sukurti.</span><span class="sxs-lookup"><span data-stu-id="4631f-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="4631f-113">Patikrinkite, ar visi sąrašai ir bibliotekos viršija 5000 elementų [sąrašo rodinio limito ribą](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , nes tai gali blokuoti svetainės šablono sukūrimą.</span><span class="sxs-lookup"><span data-stu-id="4631f-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="4631f-114">Svetainė gali naudoti per daug išteklių, todėl svetainės šablonas viršija 50 megabaito (MB) limitą.</span><span class="sxs-lookup"><span data-stu-id="4631f-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="4631f-115">Kyla problemų rodant duomenis iš sąrašo, kuris naudoja peržvalgos stulpelį.</span><span class="sxs-lookup"><span data-stu-id="4631f-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="4631f-116">Daugiau informacijos ieškokite [šablono sugeneruotas sąrašas nerodo duomenų iš tinkamo peržvalgos sąrašo "SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)".</span><span class="sxs-lookup"><span data-stu-id="4631f-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="4631f-117">Išsamesnės informacijos apie įprastas problemas ir sprendimus prašome nurodyti, [kurti ir naudoti svetainės šablonus](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="4631f-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

