---
title: pats kaip failo vardas yra geriausias
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
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800053"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4dd7c-102">Reikia Alchemy Header H1, H2's neveikia.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="4dd7c-103">Geriausios praktikos ir gairės Alchemy Authoring:</span><span class="sxs-lookup"><span data-stu-id="4dd7c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4dd7c-104">Negalima **įdėti Alchemy įžvalgos aplankuose**-tai bus pertrauka URL struktūra.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="4dd7c-105">Mes ieškome į nustatant tai.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="4dd7c-106">Aplanke **Alchemyinįžymybių** failai turi būti mažosios failų pavadinimų su brūkšnelių, tarpų ex.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="4dd7c-107">***kaip į įjungtą bylinėjimąsi***.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="4dd7c-108">Į MS. pasirinktinį lauką įtraukite taisyklės ID arba atminties srities ID iš " [Alchemy" partnerių portalo](https://alchemyportal.azurewebsites.net) .</span><span class="sxs-lookup"><span data-stu-id="4dd7c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="4dd7c-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-109">ex.</span></span> <span data-ttu-id="4dd7c-110">***ms. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="4dd7c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="4dd7c-111">Naudokite likusius metaduomenis šio failo viršuje kaip šabloną.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="4dd7c-112">" [Alchemy" partnerių portale](https://alchemyportal.azurewebsites.net)pereikite prie skyriaus **klientų įžvalgos pavadinimas:** ir naudoti, kad kaip atskaitos tašką savo H1 pavadinimas įžvalgos.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4dd7c-113">Alchemija įžvalgos turi turėti tik vieną H1 viršuje arba jie bus pertrauka gamybos.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="4dd7c-114">H2s neturi atvaizduoti tiek naudoti **paryškintu** ar kitų konvencijų reikšti atskirus skirsnius.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4dd7c-115">Tada užpildykite tekstą tekste, naudodami juodraščio medžiagą, esančią "Alchemija" taisyklės puslapio sekcijoje kliento įžvalgos</span><span class="sxs-lookup"><span data-stu-id="4dd7c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4dd7c-116">Sąrašai su ženkleliais yra puikūs</span><span class="sxs-lookup"><span data-stu-id="4dd7c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4dd7c-117">Taip pat sunumeruoti sąrašai</span><span class="sxs-lookup"><span data-stu-id="4dd7c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="4dd7c-118">**Drąsus** ir *pasvirasis* yra-OK</span><span class="sxs-lookup"><span data-stu-id="4dd7c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4dd7c-119">Nuorodos visada turėtų būti arba **"nuorodos į interneto"/išorės** arba **Deep nuorodos į UI elementai**, o ne vidaus ryšius.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="4dd7c-120">Nuotraukos šiuo metu oficialiai nepalaikomos, tačiau jos pateikiamos veiksmų plane.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="4dd7c-121">Ir tai tikrai jau šiek tiek per ilgas.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="4dd7c-122">Geriausia praktika yra apie 400 simbolių---------------------------------</span><span class="sxs-lookup"><span data-stu-id="4dd7c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4dd7c-123">Kai turinys bus paruoštas, patraukite jį į gyvą šaką.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="4dd7c-124">Tada eikite į " [Alchemy" partnerių portalą](https://alchemyportal.azurewebsites.net) ir įveskite failo pavadinimą į URL lauką.</span><span class="sxs-lookup"><span data-stu-id="4dd7c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 