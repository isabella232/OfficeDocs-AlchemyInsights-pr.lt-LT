---
title: 'tas pats kaip failo vardas yra geriausia [taisyklė #-Aprašymas]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634512"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="b800c-102">Reikia Alchemy antraštės H1, H2, neveikia.</span><span class="sxs-lookup"><span data-stu-id="b800c-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="b800c-103">Geriausia praktika ir rengti gaires Alchemija kūrimo:</span><span class="sxs-lookup"><span data-stu-id="b800c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="b800c-104">**Neįdėtas Alchemija įžvalgos aplankuose**- tai nutrauks url struktūrą.</span><span class="sxs-lookup"><span data-stu-id="b800c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="b800c-105">Mes ieškome į tvirtinimo tai.</span><span class="sxs-lookup"><span data-stu-id="b800c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="b800c-106">Failus į aplanką **AlchemyInsights** turėtų būti taisyklė ID ir taisyklės pavadinimas [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) failo vardas.</span><span class="sxs-lookup"><span data-stu-id="b800c-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="b800c-107">ex.</span><span class="sxs-lookup"><span data-stu-id="b800c-107">ex.</span></span> <span data-ttu-id="b800c-108">***976-How-to-enable-Litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="b800c-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="b800c-109">Naudoti metaduomenų šio failo viršuje jūsų šabloną.</span><span class="sxs-lookup"><span data-stu-id="b800c-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="b800c-110">Daugiau nieko nereikia.</span><span class="sxs-lookup"><span data-stu-id="b800c-110">Nothing else is required.</span></span>
1. <span data-ttu-id="b800c-111">[Alchemija partnerių portale](https://alchemyportal.azurewebsites.net)naršyti žemyn į skiltį **klientų supratimą pavadinimas:** ir naudoti, kad pradžios taškas H1 pavadinimo už supratimą.</span><span class="sxs-lookup"><span data-stu-id="b800c-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="b800c-112">Alchemija tendencijos turi turėti tik vieną H1 į viršų arba jie bus pertrauka gamybos.</span><span class="sxs-lookup"><span data-stu-id="b800c-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="b800c-113">H2s ne padaryti tiek naudoti **paryškinti** arba kitomis konvencijomis reiškia atskiruose skyriuose.</span><span class="sxs-lookup"><span data-stu-id="b800c-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="b800c-114">Be to, užpildykite naudojant projekto medžiagą įžvalgų apie klientą dalyje Alchemija taisyklė puslapio tekste</span><span class="sxs-lookup"><span data-stu-id="b800c-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="b800c-115">Sąrašai su ženkleliais yra gerai</span><span class="sxs-lookup"><span data-stu-id="b800c-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="b800c-116">Numeruotas sąrašas per</span><span class="sxs-lookup"><span data-stu-id="b800c-116">Numbered lists too</span></span>
    1. <span data-ttu-id="b800c-117">**Drąsiai** ir *kursyvas* yra OK-</span><span class="sxs-lookup"><span data-stu-id="b800c-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="b800c-118">Nuorodas visada turi būti arba **"nuorodos ä¯ interneto" / užsienio** arba **giliai nuorodos į vartotojo sąsajos elementai**, ne vidaus ryšius.</span><span class="sxs-lookup"><span data-stu-id="b800c-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="b800c-119">Ir tai tikrai jau yra šiek tiek per ilgas.</span><span class="sxs-lookup"><span data-stu-id="b800c-119">And this is really already a bit too long.</span></span> <span data-ttu-id="b800c-120">Geriausia praktika yra apie 400 simbolių---</span><span class="sxs-lookup"><span data-stu-id="b800c-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="b800c-121">Kai jūsų turinys yra pasirengusi, traukti į gyvos apatinės šakos.</span><span class="sxs-lookup"><span data-stu-id="b800c-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="b800c-122">Tada eikite į [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ir url lauke įveskite failo vardą.</span><span class="sxs-lookup"><span data-stu-id="b800c-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="b800c-123">Įsitikinkite, kad pažvelgti peržiūrėjo ir paskelbė sako "taip" ir tada spustelėkite naujinimo taisyklė.</span><span class="sxs-lookup"><span data-stu-id="b800c-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="b800c-124">**(Tai atrodys gražiau naują versiją portalas - Atleidus Netrukus).** 
 ![url lauką](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="b800c-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

