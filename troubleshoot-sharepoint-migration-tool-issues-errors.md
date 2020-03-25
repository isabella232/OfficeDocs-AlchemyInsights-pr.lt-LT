---
title: SharePoint perkėlimo įrankio trikčių diagnostika
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931126"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="94338-102">SharePoint perkėlimo įrankio trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="94338-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="94338-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="94338-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="94338-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="94338-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="94338-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="94338-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="94338-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="94338-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="94338-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="94338-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="94338-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="94338-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="94338-109">**Dažniausiai pasitaikančios problemos ir klaidos**</span><span class="sxs-lookup"><span data-stu-id="94338-109">**Common issues and errors**</span></span>

<span data-ttu-id="94338-110">Naudodami SharePoint perkėlimo įrankį (SPMT) gali kilti dažniausiai pasitaikančių problemų ir klaidų.</span><span class="sxs-lookup"><span data-stu-id="94338-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="94338-111">Norėdami gauti daugiau informacijos, perskaitykite toliau pateiktas nuorodas.</span><span class="sxs-lookup"><span data-stu-id="94338-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="94338-112">Dažniausiai pasitaikančių SPMT trikčių diagnostika ir klaidos</span><span class="sxs-lookup"><span data-stu-id="94338-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="94338-113">SPMT diegimo trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="94338-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)