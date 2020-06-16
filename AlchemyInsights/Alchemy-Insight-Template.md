---
title: tas pats kaip failo vardas yra geriausias
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750978"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="210ac-102">"Reikalinga Alchemija Antraštė H1, H2's neveikia."</span><span class="sxs-lookup"><span data-stu-id="210ac-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="210ac-103">Geriausia praktika ir gairės Alchemija kūrimo:</span><span class="sxs-lookup"><span data-stu-id="210ac-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="210ac-104">**Negalima įdėti Alchemijos įžvalgos aplankuose**- tai bus pertrauka URL struktūrą.</span><span class="sxs-lookup"><span data-stu-id="210ac-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="210ac-105">Mes ieškome, kaip tai ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="210ac-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="210ac-106">Aplanke **AlchemyInsights** esantys failai turi turėti mažąsias failų vardus su brūkšneliais tarpams.</span><span class="sxs-lookup"><span data-stu-id="210ac-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="210ac-107">***"how-to-enable-litigation-hold".***</span><span class="sxs-lookup"><span data-stu-id="210ac-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="210ac-108">Įtraukite taisyklės ID arba ieškos id iš [Alchemijos partnerių portalo](https://alchemyportal.azurewebsites.net) į lauką ms.custom.</span><span class="sxs-lookup"><span data-stu-id="210ac-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="210ac-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="210ac-109">ex.</span></span> <span data-ttu-id="210ac-110">***ms.custom: 100021 ms.custom: 100021 ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="210ac-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="210ac-111">Naudokite likusius metaduomenis šio failo viršuje kaip šabloną.</span><span class="sxs-lookup"><span data-stu-id="210ac-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="210ac-112">["Alchemy" partnerių portale](https://alchemyportal.azurewebsites.net)eikite į skyrių **Klientų įžvalgos pavadinimas:** ir naudokite tai kaip atspirties tašką savo H1 pavadinimui įžvalgai.</span><span class="sxs-lookup"><span data-stu-id="210ac-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="210ac-113">Alchemija Įžvalgos turi turėti tik vieną H1 viršuje arba jie bus pertrauka gamybos.</span><span class="sxs-lookup"><span data-stu-id="210ac-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="210ac-114">H2s netampa nei taip naudoti **paryškinti** ar kitų konvencijų reikšti atskiras sekcijas.</span><span class="sxs-lookup"><span data-stu-id="210ac-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="210ac-115">Tada užpildykite pagrindinį tekstą naudodami medžiagos juodraštį, esantį puslapio Alchemijos taisyklė skyriuje Klientų įžvalgos</span><span class="sxs-lookup"><span data-stu-id="210ac-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="210ac-116">Sąrašai su ženkleliais yra gerai</span><span class="sxs-lookup"><span data-stu-id="210ac-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="210ac-117">Taip pat sunumeruoti sąrašai</span><span class="sxs-lookup"><span data-stu-id="210ac-117">Numbered lists too</span></span>
    1. <span data-ttu-id="210ac-118">**Paryškintasis** ir *pasvirasis* yra a-ok</span><span class="sxs-lookup"><span data-stu-id="210ac-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="210ac-119">Nuorodos visada turėtų būti **arba "nuorodos į interneto" / išorės** arba **gilias nuorodas į UI elementai, o**ne vidaus nuorodos.</span><span class="sxs-lookup"><span data-stu-id="210ac-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="210ac-120">Šiuo metu nuotraukos nėra oficialiai palaikomos, tačiau jos yra veiksmų plane.</span><span class="sxs-lookup"><span data-stu-id="210ac-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="210ac-121">Ir tai tikrai jau šiek tiek per ilgas.</span><span class="sxs-lookup"><span data-stu-id="210ac-121">And this is really already a bit too long.</span></span> <span data-ttu-id="210ac-122">Geriausia praktika yra apie 400 simbolių ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="210ac-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="210ac-123">Kai jūsų turinys bus paruoštas, traukite jį į gyvą šaką.</span><span class="sxs-lookup"><span data-stu-id="210ac-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="210ac-124">Tada eikite į [Alchemijos partnerių portalą](https://alchemyportal.azurewebsites.net) ir įveskite failo vardą į url lauką.</span><span class="sxs-lookup"><span data-stu-id="210ac-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 