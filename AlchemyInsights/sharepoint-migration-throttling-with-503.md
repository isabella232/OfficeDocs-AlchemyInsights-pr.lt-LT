---
title: "\"SharePoint\" perkėlimo buferizavimas su 503 klaidomis"
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931666"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="d4c3d-102">"SharePoint" perkėlimo buferizavimas su 503 klaidomis</span><span class="sxs-lookup"><span data-stu-id="d4c3d-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="d4c3d-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d4c3d-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d4c3d-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d4c3d-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="d4c3d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d4c3d-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d4c3d-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d4c3d-109">**503 klaidos pereinant prie SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="d4c3d-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="d4c3d-110">Atrodo, kad perkeliate į "SharePoint Online" ir gaunate 503 klaidas.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="d4c3d-111">Prašome atlikti toliau nurodytus veiksmus, kad galėtume jums kuo greičiau jums padėti.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="d4c3d-112">Spustelėkite **Kreiptis į palaikymo tarnybą**, tada Nauja tarnybos **užklausa**.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="d4c3d-113">Pavadinimą ir aprašą įveskite **SharePoint perkėlimo buferizavimas su 503**.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="d4c3d-114">Kai bilietas bus pateiktas, atnaujinkite jį tokia informacija:</span><span class="sxs-lookup"><span data-stu-id="d4c3d-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="d4c3d-115">Kiek liko iš migracijos (pavyzdžiui, kiek TBs?).</span><span class="sxs-lookup"><span data-stu-id="d4c3d-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="d4c3d-116">Perkėlimo pradžios ir pabaigos data.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-116">Migration start and end date.</span></span>
    - <span data-ttu-id="d4c3d-117">Aprašykite, iš kur perkeliate turinį, pvz., "SharePoint Server", "Box", "GDrive", failų bendrinimą ir kt.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="d4c3d-118">Apskaičiuokite buferizavimo klaidų skaičių (pvz., x droselinę sklendę per valandą?) ir kada įvyksta buferizavimas.</span><span class="sxs-lookup"><span data-stu-id="d4c3d-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="d4c3d-119">Kurį perkėlimo įrankį naudojate (pvz., SPMT arba ShareGate).</span><span class="sxs-lookup"><span data-stu-id="d4c3d-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


