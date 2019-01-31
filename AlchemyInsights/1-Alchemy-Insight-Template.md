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
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662938"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="fbf9a-102">Neveikia reikia klientų susiduria su H1, H2</span><span class="sxs-lookup"><span data-stu-id="fbf9a-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="fbf9a-103">Pavyzdys teksto blokas - vadovaukitės šiomis instrukcijomis:</span><span class="sxs-lookup"><span data-stu-id="fbf9a-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="fbf9a-104">Failus į aplanką **AlchemyInsights** turėtų būti taisyklė ID ir taisyklės pavadinimas [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) failo vardas.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="fbf9a-p101">pvz ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="fbf9a-p102">Naudoti metaduomenų šio failo viršuje jūsų šabloną. Daugiau nieko nereikia.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="fbf9a-109">[Alchemija partnerių portale](https://alchemyportal.azurewebsites.net)naršyti žemyn į skiltį **klientų supratimą pavadinimas:** ir naudoti, kad pradžios taškas H1 pavadinimo už supratimą.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fbf9a-p103">Alchemija tendencijos turi turėti tik vieną H1 į viršų arba jie bus pertrauka gamybos. H2s ne padaryti tiek naudoti **paryškinti** arba kitomis konvencijomis reiškia atskiruose skyriuose.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fbf9a-112">Be to, užpildykite naudojant projekto medžiagą įžvalgų apie klientą dalyje Alchemija taisyklė puslapio tekste</span><span class="sxs-lookup"><span data-stu-id="fbf9a-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fbf9a-113">Sąrašai su ženkleliais yra gerai</span><span class="sxs-lookup"><span data-stu-id="fbf9a-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fbf9a-114">Numeruotas sąrašas per</span><span class="sxs-lookup"><span data-stu-id="fbf9a-114">Numbered lists too</span></span>
    1. <span data-ttu-id="fbf9a-115">**Drąsiai** ir *kursyvas* yra OK-</span><span class="sxs-lookup"><span data-stu-id="fbf9a-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fbf9a-116">Nuorodas visada turi būti arba **"nuorodos ä¯ interneto" / užsienio** arba **giliai nuorodos į vartotojo sąsajos elementai**, ne vidaus ryšius.</span><span class="sxs-lookup"><span data-stu-id="fbf9a-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="fbf9a-p104">Ir tai tikrai jau yra šiek tiek per ilgas. Geriausia praktika yra apie 400 simbolių---</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fbf9a-p105">Kai jūsų turinys yra pasirengusi, traukti į gyvos apatinės šakos. Tada eikite į [Alchemija partnerių portale](https://alchemyportal.azurewebsites.net) ir url lauke įveskite failo vardą. Įsitikinkite, kad pažvelgti peržiūrėjo ir paskelbė sako "taip" ir tada spustelėkite naujinimo taisyklė. (Tai atrodys gražiau naują versiją portalas - Atleidus Netrukus).</span><span class="sxs-lookup"><span data-stu-id="fbf9a-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL lauką](media/for-content-team.PNG)

