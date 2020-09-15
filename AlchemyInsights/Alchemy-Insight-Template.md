---
title: toks pat kaip failo vardas yra geriausias
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664142"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="161ee-102">"Reikalinga Alchemy antraštė H1, H2's neveikia."</span><span class="sxs-lookup"><span data-stu-id="161ee-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="161ee-103">Geriausia "Alchemy" kūrimo praktika ir gairės:</span><span class="sxs-lookup"><span data-stu-id="161ee-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="161ee-104">**Nedėkite "Alchemy" įžvalgų aplankuose**– tai nutrauks URL struktūrą.</span><span class="sxs-lookup"><span data-stu-id="161ee-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="161ee-105">Ieškome, kaip tai išspręsti.</span><span class="sxs-lookup"><span data-stu-id="161ee-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="161ee-106">Failuose, esančiame aplanke **Alchemyįžvalgos** , turi būti mažosios failų pavadinimų su brūkšneliais, skirtais tarpų ex.</span><span class="sxs-lookup"><span data-stu-id="161ee-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="161ee-107">***kaip ir įgalinti – sulaikymas dėl bylinėjimosi***.</span><span class="sxs-lookup"><span data-stu-id="161ee-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="161ee-108">Įtraukite taisyklės ID arba atminties ID iš " [Alchemy" partnerio portalo](https://alchemyportal.azurewebsites.net) , esančio lauke ms. pasirinktinio.</span><span class="sxs-lookup"><span data-stu-id="161ee-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="161ee-109">ex.</span><span class="sxs-lookup"><span data-stu-id="161ee-109">ex.</span></span> <span data-ttu-id="161ee-110">***Miss pasirinktinai: 100021***</span><span class="sxs-lookup"><span data-stu-id="161ee-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="161ee-111">Naudokite kitus metaduomenis šio failo viršuje kaip šabloną.</span><span class="sxs-lookup"><span data-stu-id="161ee-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="161ee-112">" [Alchemy" partnerio portale](https://alchemyportal.azurewebsites.net)pereikite prie skyriaus **kliento įžvalgos pavadinimas:** ir naudokite jį kaip savo H1 pavadinimo pradinį tašką.</span><span class="sxs-lookup"><span data-stu-id="161ee-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="161ee-113">"Alchemy" įžvalgų viršuje turi būti tik vienas H1 arba jie bus išskaidyti gamyboje.</span><span class="sxs-lookup"><span data-stu-id="161ee-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="161ee-114">H2s negeneruotų taip naudoti **drąsių** arba kitų konvencijų, kurios reiškia atskiras sekcijas.</span><span class="sxs-lookup"><span data-stu-id="161ee-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="161ee-115">Tada įveskite pagrindinį tekstą, naudodami medžiagos projektą "Alchemy" taisyklės puslapio sekcijoje klientų įžvalgos</span><span class="sxs-lookup"><span data-stu-id="161ee-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="161ee-116">Sąrašai su ženkleliais yra gerai</span><span class="sxs-lookup"><span data-stu-id="161ee-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="161ee-117">Sunumeruoti sąrašai irgi</span><span class="sxs-lookup"><span data-stu-id="161ee-117">Numbered lists too</span></span>
    1. <span data-ttu-id="161ee-118">**Paryškintasis** ir *pasvirasis* yra gerai</span><span class="sxs-lookup"><span data-stu-id="161ee-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="161ee-119">Saitai visada turi būti **"saitai su žiniatinkliu"/išoriniai** arba **Giluminiai saitai su vartotojo sąsajos elementais**, o ne vidiniais saitais.</span><span class="sxs-lookup"><span data-stu-id="161ee-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="161ee-120">Šiuo metu Paveikslėliai nėra oficialiai palaikomi, tačiau tai yra veiksmų planas.</span><span class="sxs-lookup"><span data-stu-id="161ee-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="161ee-121">Ir tai tikrai jau gana ilgai.</span><span class="sxs-lookup"><span data-stu-id="161ee-121">And this is really already a bit too long.</span></span> <span data-ttu-id="161ee-122">Geriausia praktika yra apie 400 simbolius---------------------------------</span><span class="sxs-lookup"><span data-stu-id="161ee-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="161ee-123">Kai turinys bus paruoštas, patraukite jį į gyvą filialą.</span><span class="sxs-lookup"><span data-stu-id="161ee-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="161ee-124">Tada eikite į " [Alchemy" partnerio portalą](https://alchemyportal.azurewebsites.net) ir įveskite failo vardą į URL lauką.</span><span class="sxs-lookup"><span data-stu-id="161ee-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 