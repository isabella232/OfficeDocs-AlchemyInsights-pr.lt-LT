---
title: Sukeisti savo Classic šaknų svetainę su šiuolaikinės svetainės
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042935"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="40f99-102">Sukeisti savo Classic šaknų svetainę su šiuolaikinės svetainės</span><span class="sxs-lookup"><span data-stu-id="40f99-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="40f99-103">Jei jūsų aplinka buvo nustatyta iki balandžio 2019 d., galite pakeisti savo šakninę svetainę į modernią svetainę naudodami "Microsoft PowerShell":</span><span class="sxs-lookup"><span data-stu-id="40f99-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="40f99-104">Jei turite kitą svetainę, kurią norite naudoti kaip savo šakninę svetainę, galite pakeisti [(keisti) šakninę svetainę](https://docs.microsoft.com/sharepoint/modern-root-site) su ja.</span><span class="sxs-lookup"><span data-stu-id="40f99-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="40f99-105">Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo vietą su kita svetaine, o archyvuojama originali svetainės vieta.</span><span class="sxs-lookup"><span data-stu-id="40f99-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="40f99-106">Pasiekiama tiek komandos svetainei (neprisijungtoms prie grupės), tiek bendravimo svetainei.</span><span class="sxs-lookup"><span data-stu-id="40f99-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="40f99-107">Netrukus bus įvesta papildomų galimybių, kurios leis jums išlaikyti naudojant svetainės turinį, bet konvertuoti esamą svetainę į komunikacijos svetainę.</span><span class="sxs-lookup"><span data-stu-id="40f99-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="40f99-108">Šios galimybės bus diegiamos palaipsniui.</span><span class="sxs-lookup"><span data-stu-id="40f99-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="40f99-109">Toliau tikrinkite "Office 365" pranešimų centro naujinimus.</span><span class="sxs-lookup"><span data-stu-id="40f99-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="40f99-110">Žinomos problemos su svetainių keitimu</span><span class="sxs-lookup"><span data-stu-id="40f99-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="40f99-111">Paskirties svetainė gali grąžinti "nerastas" (HTTP 404) klaidos trumpą laiką.</span><span class="sxs-lookup"><span data-stu-id="40f99-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="40f99-112">Turinys turi būti aptinkama atnaujinti paieškos indeksą.</span><span class="sxs-lookup"><span data-stu-id="40f99-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="40f99-113">Nėra rankinio žingsnio reikia-tai bus daroma automatiškai.</span><span class="sxs-lookup"><span data-stu-id="40f99-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="40f99-114">Viskas priklauso nuo "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) reikės rankiniu būdu ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="40f99-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="40f99-115">Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL.</span><span class="sxs-lookup"><span data-stu-id="40f99-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="40f99-116">Gaukite visų organizacinių naujienų svetainių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="40f99-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="40f99-117">"Project Server" svetaines gali reikėti patvirtinti, siekiant užtikrinti, kad jos vis dar tinkamai susietos.</span><span class="sxs-lookup"><span data-stu-id="40f99-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





