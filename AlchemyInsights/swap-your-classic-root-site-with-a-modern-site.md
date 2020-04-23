---
title: Sukeiskite savo klasikinę šakninę svetainę su modernia svetaine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741552"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="58a3c-102">Sukeiskite savo klasikinę šakninę svetainę su modernia svetaine</span><span class="sxs-lookup"><span data-stu-id="58a3c-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="58a3c-103">Jei jūsų aplinka buvo nustatyta iki 2019 m. balandžio mėn., galite pakeisti šakninę svetainę į modernią svetainę naudodami "Microsoft PowerShell":</span><span class="sxs-lookup"><span data-stu-id="58a3c-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="58a3c-104">Jei turite kitą svetainę, kurią norite naudoti kaip savo šakninę svetainę, galite pakeisti [(apsikeitimo) šakninė svetainė](https://docs.microsoft.com/sharepoint/modern-root-site) su juo.</span><span class="sxs-lookup"><span data-stu-id="58a3c-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="58a3c-105">Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pakeisti svetainės vietą su kita svetaine, o archyvuoti pradinę svetainę.</span><span class="sxs-lookup"><span data-stu-id="58a3c-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="58a3c-106">Galima naudoti ir komandos svetainėje (neprijungtoje prie grupės), ir ryšių svetainėje.</span><span class="sxs-lookup"><span data-stu-id="58a3c-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="58a3c-107">Netrukus bus įvestos papildomos galimybės, kurios leis jums toliau naudoti svetainės turinį, bet konvertuoti esamą svetainę į ryšio svetainę.</span><span class="sxs-lookup"><span data-stu-id="58a3c-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="58a3c-108">Šios galimybės bus diegiamos palaipsniui.</span><span class="sxs-lookup"><span data-stu-id="58a3c-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="58a3c-109">Toliau patikrinkite, ar pranešimų centre nėra naujinimų.</span><span class="sxs-lookup"><span data-stu-id="58a3c-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="58a3c-110">Žinomos problemos, susijusios su svetainių swapping</span><span class="sxs-lookup"><span data-stu-id="58a3c-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="58a3c-111">Paskirties svetainė gali pateikti klaidos "nerasta" (HTTP 404) trumpą laiką.</span><span class="sxs-lookup"><span data-stu-id="58a3c-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="58a3c-112">Norint atnaujinti ieškos indeksą, turinį reikės nuskaityti iš naujo.</span><span class="sxs-lookup"><span data-stu-id="58a3c-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="58a3c-113">Nėra rankinio žingsnio reikia - tai bus daroma automatiškai.</span><span class="sxs-lookup"><span data-stu-id="58a3c-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="58a3c-114">Viskas, kas priklauso nuo "statinių" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti ištaisyta rankiniu būdu.</span><span class="sxs-lookup"><span data-stu-id="58a3c-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="58a3c-115">Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL.</span><span class="sxs-lookup"><span data-stu-id="58a3c-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="58a3c-116">Gaukite visų organizacinių naujienų svetainių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="58a3c-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="58a3c-117">Project Server svetainėse gali tekti patikrinti, siekiant užtikrinti, kad jie vis dar tinkamai susiję.</span><span class="sxs-lookup"><span data-stu-id="58a3c-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
