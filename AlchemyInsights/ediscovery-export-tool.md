---
title: El. duomenų aptikimo eksportavimo įrankis
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814596"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="f641b-102">Negalite įdiegti arba paleisti el. duomenų aptikimo eksportavimo įrankio?</span><span class="sxs-lookup"><span data-stu-id="f641b-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="f641b-103">Jei negalite įdiegti arba paleisti el. duomenų aptikimo eksportavimo įrankio, kad atsisiųstumėte ieškos rezultatus, patikrinkite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="f641b-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="f641b-104">Jūsų naudojamas kompiuteris atitinka šiuos išankstinius reikalavimus:</span><span class="sxs-lookup"><span data-stu-id="f641b-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="f641b-105">32 arba 64 bitų "Windows 7" ir naujesnės versijos</span><span class="sxs-lookup"><span data-stu-id="f641b-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="f641b-106">„Microsoft .NET Framework 4.7“</span><span class="sxs-lookup"><span data-stu-id="f641b-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="f641b-107">Palaikoma naršyklė:</span><span class="sxs-lookup"><span data-stu-id="f641b-107">A supported browser:</span></span>

  - <span data-ttu-id="f641b-108">„Microsoft Edge“</span><span class="sxs-lookup"><span data-stu-id="f641b-108">Microsoft Edge</span></span>

    <span data-ttu-id="f641b-109">Arba</span><span class="sxs-lookup"><span data-stu-id="f641b-109">Or</span></span>

  - <span data-ttu-id="f641b-110">"Internet Explorer 10" ir naujesnės versijos</span><span class="sxs-lookup"><span data-stu-id="f641b-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="f641b-111">Kitos naršyklės, pvz., "Google Chrome" ir "Mozilla Firefox", nepalaikomos.</span><span class="sxs-lookup"><span data-stu-id="f641b-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="f641b-112">Jūsų organizacija gali prisijungti prie pabaigos taško "Azure", **\* kuris yra .blob.core.windows.net** (pakaitos ženklas nurodo unikalų eksportavimo užduoties identifikatorių).</span><span class="sxs-lookup"><span data-stu-id="f641b-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="f641b-113">Jums priskirtas eksportavimo vaidmuo "Microsoft 365" saugos &amp; atitikties centre.</span><span class="sxs-lookup"><span data-stu-id="f641b-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="f641b-114">Pagal numatytuosius nustatymus šis vaidmuo priskiriamas tik el. duomenų aptikimo tvarkytuvo vaidmenų grupei.</span><span class="sxs-lookup"><span data-stu-id="f641b-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="f641b-115">Žr. [El. duomenų aptikimo teisių priskyrimas](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="f641b-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="f641b-116">Daugiau informacijos žr. [Turinio ieškos rezultatų eksportavimas](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="f641b-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="f641b-117">Jei eksportuojate daugiau nei 100 K pašto dėžutes, norėdami atsisiųsti eksportavimo rezultatus, turėsite naudoti šią "Powershell": Rezultatų eksportavimas iš daugiau nei [100K pašto dėžučių.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="f641b-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>