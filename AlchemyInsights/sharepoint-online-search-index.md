---
title: Tvarkyti ieškos žodynai SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736060"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="982b3-102">Paieška: SharePoint internete</span><span class="sxs-lookup"><span data-stu-id="982b3-102">Search in SharePoint Online</span></span>

<span data-ttu-id="982b3-103">Turinys turi būti nuskaityti ir įtraukiamas į ieškos rodyklę vartotojams rasti ką jie ieško SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="982b3-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="982b3-104">Turinys automatiškai Naršoma pagal iš anksto nustatytus nuskaitymo tvarkaraštį (nuskaitymo tvarkaraštį pakeisti negalima).</span><span class="sxs-lookup"><span data-stu-id="982b3-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="982b3-105">Aptikimo robotui susitvarko turinį, kuris buvo pakeistas nuo paskutiniojo aptikimo ir atnaujina rodyklę.</span><span class="sxs-lookup"><span data-stu-id="982b3-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="982b3-106">Siekiant užtikrinti nuskaityti turinys ir rodyklė yra atnaujinama, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="982b3-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="982b3-107">Įsitikinkite, kad turinys gali būti rasti darant svetainės turinio paieškai.</span><span class="sxs-lookup"><span data-stu-id="982b3-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="982b3-108">Daugiau informacijos rasite [turinio svetainėje ieškomumo įgalinimas](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="982b3-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="982b3-109">Kai pakeičiate valdoma ypatybė arba kai pakeičiate išdėstymą, nuskaityti ir valdyti prieš keitimai atsispindės paieškos indeksą savybės, svetainės turi būti iš naujo aptiktos.</span><span class="sxs-lookup"><span data-stu-id="982b3-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="982b3-110">Nes jūsų keitimai bus atlikti ieškos schemos, o ne į faktinį svetainėje, skaitytuvas bus automatiškai iš naujo indeksuoti svetainę.</span><span class="sxs-lookup"><span data-stu-id="982b3-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="982b3-111">Daugiau informacijos ieškokite [rankiniu būdu prašymą ir iš naujo indeksuodama svetainę, biblioteka arba sąrašas](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="982b3-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="982b3-112">Palaukite bent 24 valandas po rankiniu būdu prašančioji aptikimo ir visiškai iš naujo indeksuoti Norėdami pamatyti, jei vis dar kyla klausimas.</span><span class="sxs-lookup"><span data-stu-id="982b3-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="982b3-113">Jei daugiau nei 24 valandų praėjo nuo galite pradėti nuskaityti ir visiškai iš naujo indeksuoti, prašome prisijungti palaikymo bylą.</span><span class="sxs-lookup"><span data-stu-id="982b3-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="982b3-114">Daugeliu atvejų, mes jau dirbame išeitį.</span><span class="sxs-lookup"><span data-stu-id="982b3-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="982b3-115">Nurodykite bent 24 valandas atlikti sprendimą.</span><span class="sxs-lookup"><span data-stu-id="982b3-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="982b3-116">**Svarbu žinoti**: jei svetainė, dokumentą (biblioteka) arba sąraše buvo ištrintas ir vis dar rodo paieškos rezultatus, vartotojai turėtų gauti dėl klaidos 404 Failas nerastas bandant pasiekti.</span><span class="sxs-lookup"><span data-stu-id="982b3-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="982b3-117">Ši problema turėtų būti registruojami aptarnavimo tolesnių tyrimų.</span><span class="sxs-lookup"><span data-stu-id="982b3-117">This issue should be logged as a support case for further investigation.</span></span> 



