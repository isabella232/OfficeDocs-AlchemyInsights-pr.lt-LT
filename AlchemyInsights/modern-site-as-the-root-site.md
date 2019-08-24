---
title: Modernus svetainės kaip šakninė svetainė
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620767"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="5acf6-102">Modernus svetainės kaip šakninė svetainė</span><span class="sxs-lookup"><span data-stu-id="5acf6-102">Modern site as root site</span></span>

<span data-ttu-id="5acf6-103">Mes pradėjome įdiegiant naują funkciją, kuri leis jums apsikeitimo jūsų classic svetainę šakninė svetainė su šiuolaikinės svetainės.</span><span class="sxs-lookup"><span data-stu-id="5acf6-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="5acf6-104">Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo su kita svetaine svetainės vietą, o archyvavimo originalų puslapį.</span><span class="sxs-lookup"><span data-stu-id="5acf6-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="5acf6-105">Galima komandos svetainėje (nėra prijungtas prie grupės) bei bendravimo svetainės.</span><span class="sxs-lookup"><span data-stu-id="5acf6-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="5acf6-106">Ne ištrinti savo "classic" šaknų svetainę sukurti šiuolaikinės komunikacijos svetainę.</span><span class="sxs-lookup"><span data-stu-id="5acf6-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="5acf6-107">Tai nėra palaikoma "Microsoft".</span><span class="sxs-lookup"><span data-stu-id="5acf6-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="5acf6-108">Panaikinus šakninė svetainė leis visus "SharePoint" svetainių organizacijoje neprieinama visiems naudotojams, tol, kol galite atkurti į svetainės arba sukurti naują svetainę tuo pačiu URL.</span><span class="sxs-lookup"><span data-stu-id="5acf6-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="5acf6-109">Mes bus perduoti šią funkciją per pranešimų centras.</span><span class="sxs-lookup"><span data-stu-id="5acf6-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="5acf6-110">Reikia tikėtis funkciją galima įjungti į savo nuomotojo artimiausiu metu.</span><span class="sxs-lookup"><span data-stu-id="5acf6-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="5acf6-111">Žinomos problemos su apsikeitimo svetaines</span><span class="sxs-lookup"><span data-stu-id="5acf6-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="5acf6-112">Tikslinės svetainės gali grįžti su "nerasta" klaida (HTTP 404) per trumpą laiką.</span><span class="sxs-lookup"><span data-stu-id="5acf6-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="5acf6-113">Medžiaga turi būti recrawled į paieškos indeksą atnaujinti.</span><span class="sxs-lookup"><span data-stu-id="5acf6-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="5acf6-114">Nėra jokių rankiniu būdu pirmiausia reikia čia, tai bus padaryta automatiškai.</span><span class="sxs-lookup"><span data-stu-id="5acf6-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="5acf6-115">Nieko priklauso "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) turės rankiniu būdu ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="5acf6-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="5acf6-116">Projekto serverio svetainėse gali tekti būti patikrintas siekiant užtikrinti, kad jie dar siejama teisingai.</span><span class="sxs-lookup"><span data-stu-id="5acf6-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
