---
title: Moderni svetainė kaip pagrindinė svetainė
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666878"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="1168c-102">Moderni svetainė kaip pagrindinė svetainė</span><span class="sxs-lookup"><span data-stu-id="1168c-102">Modern site as root site</span></span>

<span data-ttu-id="1168c-103">Pradėjome naudoti naują funkciją, kuri leis jums [sukeisti klasikinės svetainės šaknies svetainę su šiuolaikine svetaine](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="1168c-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="1168c-104">Naudokite funkciją [Invoke – SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Norėdami sukeisti svetainės vietą su kita svetaine archyvuodami pradinę svetainę.</span><span class="sxs-lookup"><span data-stu-id="1168c-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1168c-105">Galima naudoti ir komandos svetainėje (nėra prijungta prie grupės) ir bendravimo svetainėje.</span><span class="sxs-lookup"><span data-stu-id="1168c-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="1168c-106">Nepanaikinkite klasikinės šaknies svetainės kurdami šiuolaikinę bendravimo svetainę.</span><span class="sxs-lookup"><span data-stu-id="1168c-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="1168c-107">Tai nepalaiko "Microsoft".</span><span class="sxs-lookup"><span data-stu-id="1168c-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="1168c-108">Panaikinus svetainę, visos jūsų organizacijos "SharePoint" svetainės bus prieinamos visiems vartotojams, kol neatkursite svetainės arba sukursite naują svetainę tame pačiame URL.</span><span class="sxs-lookup"><span data-stu-id="1168c-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="1168c-109">Perduodame šią funkciją per pranešimų centrą.</span><span class="sxs-lookup"><span data-stu-id="1168c-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="1168c-110">Turėtumėte tikėtis, kad funkcija bus įjungta jūsų nuomotojuje artimiausiu metu.</span><span class="sxs-lookup"><span data-stu-id="1168c-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1168c-111">Žinomos problemos keičiant svetaines</span><span class="sxs-lookup"><span data-stu-id="1168c-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="1168c-112">Paskirties svetainė trumpą laiką gali pateikti klaidą "nerastas" (HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="1168c-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1168c-113">Turiniui atnaujinti reikia atnaujinti ieškos indeksą.</span><span class="sxs-lookup"><span data-stu-id="1168c-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1168c-114">Čia nereikia atlikti rankinio veiksmo, tai bus atlikta automatiškai.</span><span class="sxs-lookup"><span data-stu-id="1168c-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="1168c-115">Viskas, kas priklauso nuo "statinio" saitų (pvz., failų sinchronizavimo ir "OneNote" failų), turės būti rankiniu būdu pataisyta.</span><span class="sxs-lookup"><span data-stu-id="1168c-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1168c-116">"Project Server" svetaines gali reikėti patvirtinti, kad jos būtų tinkamai susietos.</span><span class="sxs-lookup"><span data-stu-id="1168c-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
