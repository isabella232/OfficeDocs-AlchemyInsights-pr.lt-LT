---
title: Perkėlimas į „SharePoint Online“ naudojant perkėlimo tvarkytuvą
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932186"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="f2db1-102">Perkėlimas į „SharePoint Online“ naudojant perkėlimo tvarkytuvą</span><span class="sxs-lookup"><span data-stu-id="f2db1-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="f2db1-103">**Svarbu**: dauguma „SharePoint Online“ ir „OneDrive“ klientų naudoja verslui svarbias taikomąsias programas, lyginant su fone veikiančia tarnyba.</span><span class="sxs-lookup"><span data-stu-id="f2db1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f2db1-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginio kopijavimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="f2db1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f2db1-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog „SharePoint Online“ ir „OneDrive“ tarnybos išliktų lengvai prieinamos ir patikimos jūsų vartotojams, kurie nuotolinio darbo scenarijuose priklauso nuo tarnybos labiau nei kada nors anksčiau.</span><span class="sxs-lookup"><span data-stu-id="f2db1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f2db1-106">Siekdami šio tikslo, pritaikėme griežtesnius apribojimus fone veikiančioms programoms (perkėlimo, DLP ir atsarginio kopijavimo sprendimų) šiokiadienių dienos valandomis.</span><span class="sxs-lookup"><span data-stu-id="f2db1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f2db1-107">Turėtumėte tikėtis, kad tuo metu šių programų pralaidumas bus labai apribotas.</span><span class="sxs-lookup"><span data-stu-id="f2db1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f2db1-108">Tačiau vakarais ir savaitgalio valandomis tame regione tarnyba bus pasirengusi apdoroti žymiai didesnį kiekį užklausų iš fone veikiančių programų.</span><span class="sxs-lookup"><span data-stu-id="f2db1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f2db1-109">**Perkėlimo tvarkytuvas**</span><span class="sxs-lookup"><span data-stu-id="f2db1-109">**Migration Manager**</span></span>

<span data-ttu-id="f2db1-110">Esantis „SharePoint“ administravimo centre, perkėlimo tvarkytuvas padės atlikti klientų sąranką ir kurti užduotis.</span><span class="sxs-lookup"><span data-stu-id="f2db1-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="f2db1-111">Galima nurodyti visuotinius arba užduoties lygio parametrus, peržiūrėti visos užduoties eigą ir atsisiųsti agreguotą suvestinę ir užduoties lygio ataskaitas.</span><span class="sxs-lookup"><span data-stu-id="f2db1-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="f2db1-112">Darbo su perkėlimo tvarkytuvu pradžia</span><span class="sxs-lookup"><span data-stu-id="f2db1-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="f2db1-113">Perkėlimo tvarkytuvo klientų sąranka</span><span class="sxs-lookup"><span data-stu-id="f2db1-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="f2db1-114">Perkėlimo tvarkytuvo parametrai</span><span class="sxs-lookup"><span data-stu-id="f2db1-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
