---
title: "\"SharePoint Online\" užklausų buferizavimas"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931450"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5b002-102">"SharePoint Online" užklausų buferizavimas</span><span class="sxs-lookup"><span data-stu-id="5b002-102">SharePoint Online throttling</span></span>

<span data-ttu-id="5b002-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="5b002-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5b002-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="5b002-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5b002-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="5b002-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5b002-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="5b002-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5b002-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="5b002-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5b002-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="5b002-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5b002-109">**"SharePoint Online" užklausų buferizavimas**</span><span class="sxs-lookup"><span data-stu-id="5b002-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="5b002-110">"SharePoint Online" naudoja buferizavimas, kad išlaikytų optimalų "SharePoint Online" paslaugos našumą ir patikimumą.</span><span class="sxs-lookup"><span data-stu-id="5b002-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5b002-111">Buferizavimas riboja vartotojo veiksmų arba vienu metu skambučių skaičių (pagal scenarijų arba kodą), kad būtų išvengta per daug išteklių.</span><span class="sxs-lookup"><span data-stu-id="5b002-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5b002-112">Norėdami gauti daugiau informacijos, apsilankykite žemiau pateiktose nuorodose.</span><span class="sxs-lookup"><span data-stu-id="5b002-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="5b002-113">"SharePoint Online" neužblokavo arba neužblokavo</span><span class="sxs-lookup"><span data-stu-id="5b002-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="5b002-114">Duomenų perkėlimas ir SPO buferizavimas</span><span class="sxs-lookup"><span data-stu-id="5b002-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="5b002-115">"SharePoint Online" ir "OneDrive" perkėlimo greitis</span><span class="sxs-lookup"><span data-stu-id="5b002-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="5b002-116">"SharePoint Online" užklausų buferizavimas naudojant eksponentinį atgal</span><span class="sxs-lookup"><span data-stu-id="5b002-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="5b002-117">Pajėgumų planavimas ir apkrovos testavimas "SharePoint Online"</span><span class="sxs-lookup"><span data-stu-id="5b002-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

