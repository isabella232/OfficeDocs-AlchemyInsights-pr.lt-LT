---
title: pats, kaip failo vardas yra geriausias
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762072"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="3b832-102">Reikia Alchemy antraštės H1, H2, neveikia.</span><span class="sxs-lookup"><span data-stu-id="3b832-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="3b832-103">Geriausia praktika ir rengti gaires Alchemija kūrimo:</span><span class="sxs-lookup"><span data-stu-id="3b832-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="3b832-104">**Neįdėtas Alchemija įžvalgos aplankuose**- tai nutrauks url struktūrą.</span><span class="sxs-lookup"><span data-stu-id="3b832-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="3b832-105">Mes ieškome į tvirtinimo tai.</span><span class="sxs-lookup"><span data-stu-id="3b832-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="3b832-106">Failus į aplanką **AlchemyInsights** turėtų būti mažoji raidė failų vardai su brūkšneliais erdves ex.</span><span class="sxs-lookup"><span data-stu-id="3b832-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="3b832-107">***pažangiąja-į-įgalinti--sulaikymas***.</span><span class="sxs-lookup"><span data-stu-id="3b832-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="3b832-108">Įtraukti taisyklė ID arba kibiras ID [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ms.custom srityje.</span><span class="sxs-lookup"><span data-stu-id="3b832-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="3b832-109">ex.</span><span class="sxs-lookup"><span data-stu-id="3b832-109">ex.</span></span> <span data-ttu-id="3b832-110">***ms.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="3b832-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="3b832-111">Naudoti metaduomenų likusioje šio failo viršuje jūsų šabloną.</span><span class="sxs-lookup"><span data-stu-id="3b832-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="3b832-112">[Alchemija partnerių portale](https://alchemyportal.azurewebsites.net)naršyti žemyn į skiltį **klientų supratimą pavadinimas:** ir naudoti, kad pradžios taškas H1 pavadinimo už supratimą.</span><span class="sxs-lookup"><span data-stu-id="3b832-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="3b832-113">Alchemija tendencijos turi turėti tik vieną H1 į viršų arba jie bus pertrauka gamybos.</span><span class="sxs-lookup"><span data-stu-id="3b832-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="3b832-114">H2s ne padaryti tiek naudoti **paryškinti** arba kitomis konvencijomis reiškia atskiruose skyriuose.</span><span class="sxs-lookup"><span data-stu-id="3b832-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="3b832-115">Be to, užpildykite naudojant projekto medžiagą įžvalgų apie klientą dalyje Alchemija taisyklė puslapio tekste</span><span class="sxs-lookup"><span data-stu-id="3b832-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="3b832-116">Sąrašai su ženkleliais yra gerai</span><span class="sxs-lookup"><span data-stu-id="3b832-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="3b832-117">Numeruotas sąrašas per</span><span class="sxs-lookup"><span data-stu-id="3b832-117">Numbered lists too</span></span>
    1. <span data-ttu-id="3b832-118">**Drąsiai** ir *kursyvas* yra OK-</span><span class="sxs-lookup"><span data-stu-id="3b832-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="3b832-119">Nuorodas visada turi būti arba **"nuorodos ä¯ interneto" / užsienio** arba **giliai nuorodos į vartotojo sąsajos elementai**, ne vidaus ryšius.</span><span class="sxs-lookup"><span data-stu-id="3b832-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="3b832-120">Nuotraukos nėra oficialiai palaikoma šiuo metu, bet tai dėl plano.</span><span class="sxs-lookup"><span data-stu-id="3b832-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="3b832-121">Ir tai tikrai jau yra šiek tiek per ilgas.</span><span class="sxs-lookup"><span data-stu-id="3b832-121">And this is really already a bit too long.</span></span> <span data-ttu-id="3b832-122">Geriausia praktika yra apie 400 simbolių---</span><span class="sxs-lookup"><span data-stu-id="3b832-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="3b832-123">Kai jūsų turinys yra pasirengusi, traukti į gyvos apatinės šakos.</span><span class="sxs-lookup"><span data-stu-id="3b832-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="3b832-124">Tada eikite į [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ir url lauke įveskite failo vardą.</span><span class="sxs-lookup"><span data-stu-id="3b832-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="3b832-125">M</span><span class="sxs-lookup"><span data-stu-id="3b832-125">M</span></span>