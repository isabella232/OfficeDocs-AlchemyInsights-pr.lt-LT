---
title: "\"SharePoint Online\" užklausų buferizavimas"
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931234"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="a8c09-102">"SharePoint Online" užklausų buferizavimas</span><span class="sxs-lookup"><span data-stu-id="a8c09-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="a8c09-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="a8c09-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a8c09-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="a8c09-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a8c09-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="a8c09-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a8c09-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="a8c09-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a8c09-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="a8c09-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a8c09-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="a8c09-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a8c09-109">**503 serveris užimtas klaida**</span><span class="sxs-lookup"><span data-stu-id="a8c09-109">**503 server is busy error**</span></span>

<span data-ttu-id="a8c09-110">Vartotojai gali gauti 503 serveris yra užimtas klaida bandant pereiti į SharePoint "arba" OneDrive svetainėse.</span><span class="sxs-lookup"><span data-stu-id="a8c09-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="a8c09-111">Šią klaidą gali sukelti buferizavimas SharePoint tarnyboje.</span><span class="sxs-lookup"><span data-stu-id="a8c09-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a8c09-112">"SharePoint Online" naudoja buferizavimas, kad išlaikytų optimalų "SharePoint Online" paslaugos našumą ir patikimumą.</span><span class="sxs-lookup"><span data-stu-id="a8c09-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a8c09-113">Buferizavimas riboja vartotojo veiksmų arba vienu metu skambučių skaičių (pagal scenarijų arba kodą), kad būtų išvengta per daug išteklių.</span><span class="sxs-lookup"><span data-stu-id="a8c09-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="a8c09-114">Jei norite gauti daugiau informacijos apie buferizavimas [pamatyti, Išvengti gauti throttled arba užblokuotas SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="a8c09-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="a8c09-115">Jei manote, kad ši klaida nėra susijusi su buferizavimas, galite patikrinti, ar yra aktyvi priežiūra vyksta jūsų nuomotojo keliaudami į [pranešimų centrą](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="a8c09-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="a8c09-116">Galiausiai įsitikinkite, kad lankotės [puslapyje Tarnybos sveikata](https://portal.office.com/adminportal/home#/servicehealth) ir patikrinkite, ar nėra patarimų / incidentų, kurie gali įvykti.</span><span class="sxs-lookup"><span data-stu-id="a8c09-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

