---
title: „SharePoint“ perkėlimo našumas
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932242"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="38b1c-102">„SharePoint“ perkėlimo našumas</span><span class="sxs-lookup"><span data-stu-id="38b1c-102">SharePoint migration performance</span></span>

<span data-ttu-id="38b1c-103">**Svarbu**: dauguma „SharePoint Online“ ir „OneDrive“ klientų naudoja verslui svarbias taikomąsias programas, lyginant su fone veikiančia tarnyba.</span><span class="sxs-lookup"><span data-stu-id="38b1c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="38b1c-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginio kopijavimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="38b1c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="38b1c-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog „SharePoint Online“ ir „OneDrive“ tarnybos išliktų lengvai prieinamos ir patikimos jūsų vartotojams, kurie nuotolinio darbo scenarijuose priklauso nuo tarnybos labiau nei kada nors anksčiau.</span><span class="sxs-lookup"><span data-stu-id="38b1c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="38b1c-106">Siekdami šio tikslo, pritaikėme griežtesnius apribojimus fone veikiančioms programoms (perkėlimo, DLP ir atsarginio kopijavimo sprendimų) šiokiadienių dienos valandomis.</span><span class="sxs-lookup"><span data-stu-id="38b1c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="38b1c-107">Turėtumėte tikėtis, kad tuo metu šių programų pralaidumas bus labai apribotas.</span><span class="sxs-lookup"><span data-stu-id="38b1c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="38b1c-108">Tačiau vakarais ir savaitgalio valandomis tame regione tarnyba bus pasirengusi apdoroti žymiai didesnį kiekį užklausų iš fone veikiančių programų.</span><span class="sxs-lookup"><span data-stu-id="38b1c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="38b1c-109">**Perkėlimo našumas**</span><span class="sxs-lookup"><span data-stu-id="38b1c-109">**Migration performance**</span></span>

<span data-ttu-id="38b1c-110">Perkėlimo našumui įtakos gali turėti tinklo infrastruktūra, failo dydis, perkėlimo laikas ir ribojimas.</span><span class="sxs-lookup"><span data-stu-id="38b1c-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="38b1c-111">Tai suprasdami, galėsite lengviau planuoti ir maksimaliai padidinti perkėlimo efektyvumą.</span><span class="sxs-lookup"><span data-stu-id="38b1c-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="38b1c-112">Daugiau informacijos žr. toliau pateiktuose saituose.</span><span class="sxs-lookup"><span data-stu-id="38b1c-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="38b1c-113">„SharePoint Online“ ir ODB perkėlimo greitis</span><span class="sxs-lookup"><span data-stu-id="38b1c-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="38b1c-114">Išvenkite ribojimo arba blokavimo „SharePoint Online“</span><span class="sxs-lookup"><span data-stu-id="38b1c-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="38b1c-115">„SharePoint“ perkėlimo įrankio atsisiuntimas ir diegimas</span><span class="sxs-lookup"><span data-stu-id="38b1c-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
