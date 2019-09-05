---
title: Šiuolaikinė svetainė kaip šakninė svetainė
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
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753912"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="204e5-102">Šiuolaikinė svetainė kaip šakninė svetainė</span><span class="sxs-lookup"><span data-stu-id="204e5-102">Modern site as root site</span></span>

<span data-ttu-id="204e5-103">Mes pradėjome rida naują funkciją, kuri leis jums [apsikeitimo savo Classic svetainę šaknų svetainę su modernia svetaine](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="204e5-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="204e5-104">Naudokite [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) apsikeitimo vietą su kita svetaine, o archyvuojama originali svetainės vieta.</span><span class="sxs-lookup"><span data-stu-id="204e5-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="204e5-105">Pasiekiama tiek komandos svetainei (neprisijungtoms prie grupės), tiek bendravimo svetainei.</span><span class="sxs-lookup"><span data-stu-id="204e5-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="204e5-106">Nenaikinkite savo klasikinės Šakninės svetainės, kad sukurtumėte modernią bendravimo svetainę.</span><span class="sxs-lookup"><span data-stu-id="204e5-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="204e5-107">Tai nepalaiko Microsoft.</span><span class="sxs-lookup"><span data-stu-id="204e5-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="204e5-108">Panaikinus šakninę svetainę visos organizacijos SharePoint svetainės bus neprieinamos visiems vartotojams, kol neatkursite svetainės arba nesukursite naujos svetainės tuo pačiu URL.</span><span class="sxs-lookup"><span data-stu-id="204e5-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="204e5-109">Mes susisieksime su šia funkcija per pranešimų centrą.</span><span class="sxs-lookup"><span data-stu-id="204e5-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="204e5-110">Turėtumėte tikėtis, kad funkcija turi būti įjungtas jūsų nuomininkas netrukus.</span><span class="sxs-lookup"><span data-stu-id="204e5-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="204e5-111">Žinomos problemos su svetainių keitimu</span><span class="sxs-lookup"><span data-stu-id="204e5-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="204e5-112">Paskirties svetainė gali grąžinti "nerastas" (HTTP 404) klaidos trumpą laiką.</span><span class="sxs-lookup"><span data-stu-id="204e5-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="204e5-113">Turinys turi būti aptinkama atnaujinti paieškos indeksą.</span><span class="sxs-lookup"><span data-stu-id="204e5-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="204e5-114">Nėra rankinio žingsnio reikia čia, tai bus daroma automatiškai.</span><span class="sxs-lookup"><span data-stu-id="204e5-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="204e5-115">Viskas priklauso nuo "statinis" nuorodos (pvz., failų sinchronizavimo ir "OneNote" failus) reikės rankiniu būdu ištaisyti.</span><span class="sxs-lookup"><span data-stu-id="204e5-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="204e5-116">"Project Server" svetaines gali reikėti patvirtinti, siekiant užtikrinti, kad jos vis dar tinkamai susietos.</span><span class="sxs-lookup"><span data-stu-id="204e5-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
