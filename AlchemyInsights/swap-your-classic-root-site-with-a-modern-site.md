---
title: Klasikinės šaknies svetainės keitimas naudojant šiuolaikinę svetainę
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691187"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="20c94-102">Klasikinės šaknies svetainės keitimas naudojant šiuolaikinę svetainę</span><span class="sxs-lookup"><span data-stu-id="20c94-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="20c94-103">Jei jūsų aplinka buvo nustatyta iki balandžio 2019, galite pakeisti savo šaknies svetainę į šiuolaikinę svetainę naudodami "Microsoft PowerShell":</span><span class="sxs-lookup"><span data-stu-id="20c94-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="20c94-104">Jei turite kitą svetainę, kurią norite naudoti kaip savo šaknies svetainę, galite pakeisti [(sukeisti) šaknies svetainę](https://docs.microsoft.com/sharepoint/modern-root-site) su ja.</span><span class="sxs-lookup"><span data-stu-id="20c94-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="20c94-105">Naudokite funkciją [Invoke – SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Norėdami sukeisti svetainės vietą su kita svetaine archyvuodami pradinę svetainę.</span><span class="sxs-lookup"><span data-stu-id="20c94-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="20c94-106">Galima naudoti ir komandos svetainėje (nėra prijungta prie grupės) ir bendravimo svetainėje.</span><span class="sxs-lookup"><span data-stu-id="20c94-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="20c94-107">Netrukus bus įdiegtos papildomos galimybės, leidžiančios toliau naudoti svetainės turinį, bet konvertuoti esamą svetainę į ryšių svetainę.</span><span class="sxs-lookup"><span data-stu-id="20c94-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="20c94-108">Šie pajėgumai bus palaipsniui išskleidžiami.</span><span class="sxs-lookup"><span data-stu-id="20c94-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="20c94-109">Toliau tikrinkite naujinimų centro naujinimus.</span><span class="sxs-lookup"><span data-stu-id="20c94-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="20c94-110">Žinomos problemos keičiant svetaines</span><span class="sxs-lookup"><span data-stu-id="20c94-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="20c94-111">Paskirties svetainė trumpą laiką gali pateikti klaidą "nerastas" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="20c94-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="20c94-112">Turiniui atnaujinti reikia atnaujinti ieškos indeksą.</span><span class="sxs-lookup"><span data-stu-id="20c94-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="20c94-113">Nėra reikalingo rankinio veiksmo – tai bus atlikta automatiškai.</span><span class="sxs-lookup"><span data-stu-id="20c94-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="20c94-114">Viskas, kas priklauso nuo "statinio" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti rankiniu būdu pataisyta.</span><span class="sxs-lookup"><span data-stu-id="20c94-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="20c94-115">Jei šaltinio svetainė buvo organizacijos naujienų svetainė, atnaujinkite URL.</span><span class="sxs-lookup"><span data-stu-id="20c94-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="20c94-116">Gaukite visų organizacijos naujienų svetainių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="20c94-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="20c94-117">"Project Server" svetaines gali reikėti patvirtinti, kad jos būtų tinkamai susietos.</span><span class="sxs-lookup"><span data-stu-id="20c94-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
