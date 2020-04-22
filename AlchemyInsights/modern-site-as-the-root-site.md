---
title: Šiuolaikinė svetainė kaip šakninė svetainė
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713799"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="6e6d2-102">Šiuolaikinė svetainė kaip šakninė svetainė</span><span class="sxs-lookup"><span data-stu-id="6e6d2-102">Modern site as root site</span></span>

<span data-ttu-id="6e6d2-103">Mes pradėjome diegti naują funkciją, kuri leis jums [apsikeitimo savo klasikinę svetainę šaknies svetainę su modernia svetaine.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="6e6d2-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="6e6d2-104">Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pakeisti svetainės vietą su kita svetaine, o archyvuoti pradinę svetainę.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="6e6d2-105">Galima naudoti ir komandos svetainėje (neprijungtoje prie grupės), ir ryšių svetainėje.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="6e6d2-106">Neištrinkite savo klasikinės šaknies svetainės, kad sukurtumėte modernią komunikacijos svetainę.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="6e6d2-107">"Microsoft" to nepalaiko.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="6e6d2-108">Panaikinus šakninę svetainę visos jūsų organizacijos "SharePoint" svetainės taps nepasiekiamos visiems vartotojams, kol atkursite svetainę arba sukursite naują svetainę tuo pačiu URL.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="6e6d2-109">Mes bendrauti šią funkciją per pranešimų centrą.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="6e6d2-110">Turėtumėte tikėtis, kad funkcija bus įjungta jūsų nuomotojo netrukus.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="6e6d2-111">Žinomos problemos, susijusios su svetainių swapping</span><span class="sxs-lookup"><span data-stu-id="6e6d2-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="6e6d2-112">Paskirties svetainė gali pateikti klaidos "nerasta" (HTTP 404) trumpą laiką.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="6e6d2-113">Norint atnaujinti ieškos indeksą, turinį reikės nuskaityti iš naujo.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="6e6d2-114">Čia nereikia rankinio žingsnio, tai bus daroma automatiškai.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="6e6d2-115">Viskas, kas priklauso nuo "statinių" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti ištaisyta rankiniu būdu.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="6e6d2-116">Project Server svetainėse gali tekti patikrinti, siekiant užtikrinti, kad jie vis dar tinkamai susiję.</span><span class="sxs-lookup"><span data-stu-id="6e6d2-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
