---
title: Ieška "SharePoint Online"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044051"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="f28ac-102">Turinio nuskaitymas ir indeksavimas "SharePoint Online"</span><span class="sxs-lookup"><span data-stu-id="f28ac-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="f28ac-103">Turinys turi būti nuskaityti ir įtraukti į paieškos indeksą vartotojams rasti tai, ko jie ieško SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f28ac-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="f28ac-104">Turinys automatiškai aptinkamas pagal iš anksto nustatytą aptikimo grafiką (negalima keisti aptikimo grafiko).</span><span class="sxs-lookup"><span data-stu-id="f28ac-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="f28ac-105">Aptikimo robotas paima turinį, kuris pasikeitė nuo paskutinio aptikimo ir atnaujina indeksą.</span><span class="sxs-lookup"><span data-stu-id="f28ac-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="f28ac-106">Kad turinys būtų aptinkamas ir indeksas būtų atnaujintas, Įsidėmėkite:</span><span class="sxs-lookup"><span data-stu-id="f28ac-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="f28ac-107">Įsitikinkite, kad turinio galima rasti [svetainės turinio paieškai](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f28ac-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="f28ac-108">Pakeitus valdomą ypatybę arba pakeitus aptiktų ir valdomų ypatybių susiejimą, svetainė turi būti iš naujo nuskaitytas prieš tai, kai jūsų keitimai atsispindės Ieškos rodyklėje.</span><span class="sxs-lookup"><span data-stu-id="f28ac-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="f28ac-109">Kadangi jūsų pakeitimai atliekami ieškos schemoje, o ne faktinei svetainei, šliaužiklis automatiškai iš naujo neindeksuoja svetainės.</span><span class="sxs-lookup"><span data-stu-id="f28ac-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="f28ac-110">Norėdami gauti daugiau informacijos, žr [rankiniu būdu prašyti nuskaityti ir iš naujo indeksuoti svetainę, biblioteką ar sąrašą](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="f28ac-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="f28ac-111">Palaukite bent 24 valandas po to, kai rankiniu būdu prašyti nuskaitymo ir visiškai iš naujo indeksas pamatyti, jei jūs vis dar susiduria su problema.</span><span class="sxs-lookup"><span data-stu-id="f28ac-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="f28ac-112">Jei praėjo daugiau nei 24 valandos nuo tada, kai inicijavote aptikimą ir visą indeksą, prašome prisijungti prie palaikymo atvejo.</span><span class="sxs-lookup"><span data-stu-id="f28ac-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="f28ac-113">Daugeliu atvejų jau dirbame su sprendimu.</span><span class="sxs-lookup"><span data-stu-id="f28ac-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f28ac-114">Prašome pateikti mums bent 24 valandas, kad užbaigtumėte sprendimą.</span><span class="sxs-lookup"><span data-stu-id="f28ac-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f28ac-115">Jei svetainėje, dokumentas (biblioteka) arba sąrašas buvo panaikintas ir vis dar rodomas ieškos rezultatuose, vartotojai turėtų gauti **klaidos 404 failą nerastas** bandant jį pasiekti.</span><span class="sxs-lookup"><span data-stu-id="f28ac-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="f28ac-116">Šis klausimas turėtų būti registruojamas kaip paramos atvejis tolesniam tyrimui.</span><span class="sxs-lookup"><span data-stu-id="f28ac-116">This issue should be logged as a support case for further investigation.</span></span> 



