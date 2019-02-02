---
title: 'tas pats kaip failo vardas yra geriausia [taisyklė #-Aprašymas]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697138"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="ca331-102">Reikia Alchemy antraštės H1, H2, neveikia.</span><span class="sxs-lookup"><span data-stu-id="ca331-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="ca331-103">Geriausia praktika ir rengti gaires Alchemija kūrimo:</span><span class="sxs-lookup"><span data-stu-id="ca331-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="ca331-p101">**Neįdėtas Alchemija įžvalgos aplankuose**- tai nutrauks url struktūrą. Mes ieškome į tvirtinimo tai.</span><span class="sxs-lookup"><span data-stu-id="ca331-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="ca331-106">Failus į aplanką **AlchemyInsights** turėtų būti taisyklė ID ir taisyklės pavadinimas [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) failo vardas.</span><span class="sxs-lookup"><span data-stu-id="ca331-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="ca331-p102">pvz ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="ca331-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="ca331-p103">Naudoti metaduomenų šio failo viršuje jūsų šabloną. Daugiau nieko nereikia.</span><span class="sxs-lookup"><span data-stu-id="ca331-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="ca331-111">[Alchemija partnerių portale](https://alchemyportal.azurewebsites.net)naršyti žemyn į skiltį **klientų supratimą pavadinimas:** ir naudoti, kad pradžios taškas H1 pavadinimo už supratimą.</span><span class="sxs-lookup"><span data-stu-id="ca331-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ca331-p104">Alchemija tendencijos turi turėti tik vieną H1 į viršų arba jie bus pertrauka gamybos. H2s ne padaryti tiek naudoti **paryškinti** arba kitomis konvencijomis reiškia atskiruose skyriuose.</span><span class="sxs-lookup"><span data-stu-id="ca331-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ca331-114">Be to, užpildykite naudojant projekto medžiagą įžvalgų apie klientą dalyje Alchemija taisyklė puslapio tekste</span><span class="sxs-lookup"><span data-stu-id="ca331-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ca331-115">Sąrašai su ženkleliais yra gerai</span><span class="sxs-lookup"><span data-stu-id="ca331-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ca331-116">Numeruotas sąrašas per</span><span class="sxs-lookup"><span data-stu-id="ca331-116">Numbered lists too</span></span>
    1. <span data-ttu-id="ca331-117">**Drąsiai** ir *kursyvas* yra OK-</span><span class="sxs-lookup"><span data-stu-id="ca331-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ca331-118">Nuorodas visada turi būti arba **"nuorodos ä¯ interneto" / užsienio** arba **giliai nuorodos į vartotojo sąsajos elementai**, ne vidaus ryšius.</span><span class="sxs-lookup"><span data-stu-id="ca331-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="ca331-p105">Ir tai tikrai jau yra šiek tiek per ilgas. Geriausia praktika yra apie 400 simbolių---</span><span class="sxs-lookup"><span data-stu-id="ca331-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="ca331-p106">Kai jūsų turinys yra pasirengusi, traukti į gyvos apatinės šakos. Tada eikite į [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ir url lauke įveskite failo vardą. Įsitikinkite, kad pažvelgti peržiūrėjo ir paskelbė sako "taip" ir tada spustelėkite naujinimo taisyklė. **(Tai atrodys gražiau naują versiją portalas - Atleidus Netrukus).** 
 ![url lauką](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="ca331-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

