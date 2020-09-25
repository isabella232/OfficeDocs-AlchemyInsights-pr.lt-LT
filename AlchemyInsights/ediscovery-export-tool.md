---
title: "\"Udiscovery\" eksportavimo įrankis"
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277922"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="c1571-102">Nepavyksta įdiegti arba paleisti "Udiscovery" eksportavimo įrankio?</span><span class="sxs-lookup"><span data-stu-id="c1571-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="c1571-103">Jei negalite įdiegti arba paleisti "Udiscovery" eksportavimo įrankio, kad atsisiųstumėte ieškos rezultatus, patikrinkite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="c1571-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="c1571-104">Jūsų naudojamas kompiuteris atitinka šias išankstines sąlygas:</span><span class="sxs-lookup"><span data-stu-id="c1571-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="c1571-105">"32" arba "64" bitų versijos "Windows 7" ir naujesnėse versijose</span><span class="sxs-lookup"><span data-stu-id="c1571-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="c1571-106">„Microsoft .NET Framework 4.7“</span><span class="sxs-lookup"><span data-stu-id="c1571-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="c1571-107">Palaikoma naršyklė:</span><span class="sxs-lookup"><span data-stu-id="c1571-107">A supported browser:</span></span>

  - <span data-ttu-id="c1571-108">"Microsoft Edge"</span><span class="sxs-lookup"><span data-stu-id="c1571-108">Microsoft Edge</span></span>

    <span data-ttu-id="c1571-109">Arba</span><span class="sxs-lookup"><span data-stu-id="c1571-109">Or</span></span>

  - <span data-ttu-id="c1571-110">"Internet Explorer 10" ir vėlesnės versijos</span><span class="sxs-lookup"><span data-stu-id="c1571-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="c1571-111">Kitos naršyklės, pvz., "Google Chrome" ir "Mozilla Firefox", yra nepalaikomos.</span><span class="sxs-lookup"><span data-stu-id="c1571-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="c1571-112">Jūsų organizacija gali prisijungti prie galinio punkto "Azure", kuris yra \*\* \* . BLOB.Core.Windows.net\*\* (pakaitos simbolis nurodo unikalų jūsų eksportavimo užduoties identifikatorių).</span><span class="sxs-lookup"><span data-stu-id="c1571-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="c1571-113">"Microsoft 365" saugos atitikties centre priskirtas eksportavimo vaidmuo &amp; .</span><span class="sxs-lookup"><span data-stu-id="c1571-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="c1571-114">Pagal numatytuosius numatytuosius reikšmę šis vaidmuo priskiriamas tik "Udiscovery Manager" vaidmenų grupei.</span><span class="sxs-lookup"><span data-stu-id="c1571-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="c1571-115">Žiūrėkite [priskirti elektroninės aptikimo teises](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="c1571-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="c1571-116">Daugiau informacijos ieškokite [turinio ieškos rezultatų eksportavimas](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="c1571-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="c1571-117">Jei eksportuojate daugiau nei 100 k pašto dėžučių, turite naudoti šį "PowerShell", kad atsisiųstumėte eksportavimo rezultatus:  [rezultatų eksportavimas iš daugiau nei 100 k pašto dėžučių](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="c1571-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>