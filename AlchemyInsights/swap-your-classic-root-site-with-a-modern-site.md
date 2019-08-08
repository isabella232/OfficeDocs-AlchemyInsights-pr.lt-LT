---
title: Apsikeitimo savo klasikinis šakninė svetainė su moderni svetainė
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246029"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="85c3f-102">Apsikeitimo savo klasikinis šakninė svetainė su moderni svetainė</span><span class="sxs-lookup"><span data-stu-id="85c3f-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="85c3f-103">Jei jūsų aplinkoje buvo nustatytas iki 2019 m. balandžio, galite pakeisti savo šakninėje svetainėje prie šiuolaikinės svetainės naudodami Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="85c3f-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="85c3f-104">Jei turite kitą svetainę, kurią norite naudoti kaip šakninę svetainę, galite pakeisti (apsikeitimo) šaknis svetainę su juo.</span><span class="sxs-lookup"><span data-stu-id="85c3f-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="85c3f-105">Naudokite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo su kita svetaine svetainės vietą, o archyvavimo originalų puslapį.</span><span class="sxs-lookup"><span data-stu-id="85c3f-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="85c3f-106">Galima komandos svetainėje (nėra prijungtas prie grupės) bei bendravimo svetainės.</span><span class="sxs-lookup"><span data-stu-id="85c3f-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="85c3f-107">Papildomus pajėgumus pradės veikti greitai, leis jums išlaikyti naudojant turinio svetainėje, bet ir konvertuoti esamą svetainę pranešimas svetainė.</span><span class="sxs-lookup"><span data-stu-id="85c3f-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="85c3f-108">Šie pajėgumai bus diegiamos palaipsniui.</span><span class="sxs-lookup"><span data-stu-id="85c3f-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="85c3f-109">Ir toliau tikrins, ar yra naujinimų Office 365 pranešimų centras.</span><span class="sxs-lookup"><span data-stu-id="85c3f-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="85c3f-110">Žinomos problemos su apsikeitimo svetaines</span><span class="sxs-lookup"><span data-stu-id="85c3f-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="85c3f-111">Tikslinės svetainės gali grįžti su "nerasta" klaida (HTTP 404) per trumpą laiką.</span><span class="sxs-lookup"><span data-stu-id="85c3f-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="85c3f-112">Medžiaga turi būti recrawled į paieškos indeksą atnaujinti.</span><span class="sxs-lookup"><span data-stu-id="85c3f-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="85c3f-113">Nėra jokių rankiniu būdu pirmiausia reikia - tai bus padaryta automatiškai.</span><span class="sxs-lookup"><span data-stu-id="85c3f-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="85c3f-114">Nieko priklauso "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) turės rankiniu būdu ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="85c3f-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="85c3f-115">Jei šaltinio svetainė buvo organizacijos naujienų svetainę, atnaujinti URL.</span><span class="sxs-lookup"><span data-stu-id="85c3f-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="85c3f-116">Gauti visus organizacinius naujienų svetainių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="85c3f-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="85c3f-117">Projekto serverio svetainėse gali tekti būti patikrintas siekiant užtikrinti, kad jie dar siejama teisingai.</span><span class="sxs-lookup"><span data-stu-id="85c3f-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





