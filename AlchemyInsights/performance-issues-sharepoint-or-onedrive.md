---
title: Našumo problemos – "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068418"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="efc94-102">"SharePoint" arba "OneDrive" veikia lėtai, nepasiekiama arba nepasiekiama keliems vartotojams</span><span class="sxs-lookup"><span data-stu-id="efc94-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="efc94-103">SharePoint arba OneDrive gali būti lėtas, nepasiekiamas arba nepasiekiamas, arba gali Rodyti paslaugos nepasiekiamas arba 503 klaidos, dėl kelių priežasčių:</span><span class="sxs-lookup"><span data-stu-id="efc94-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="efc94-104">Jei SharePoint arba "OneDrive" svetainė yra lėta arba uždelsta keliems vartotojams, gali būti laikina paslaugų problema, dėl kurios vartotojai patiria pertrūkiais uždelsimą arba naršymo klaidas, kai pasiekiate "SharePoint" svetaines arba "OneDrive" turinį.</span><span class="sxs-lookup"><span data-stu-id="efc94-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="efc94-105">Patikrinkite [tarnybos sveikatos ataskaitų sritį](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ir pažiūrėkite, ar jūsų organizacija turi įtakos.</span><span class="sxs-lookup"><span data-stu-id="efc94-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="efc94-106">Vartotojai gali gauti *503 serverio yra užimtas* klaida bandant pereiti prie SharePoint arba OneDrive svetainių.</span><span class="sxs-lookup"><span data-stu-id="efc94-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="efc94-107">Ši klaida gali kilti dėl buferinės per SharePoint tarnybos.</span><span class="sxs-lookup"><span data-stu-id="efc94-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="efc94-108">SharePoint Online naudoja buferizavimo išlaikyti optimalų efektyvumą ir patikimumą SharePoint Online paslaugos.</span><span class="sxs-lookup"><span data-stu-id="efc94-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="efc94-109">Buferinis ribojimas riboja vartotojo veiksmų arba vienu metu vykstančių skambučių skaičių (pagal scenarijų arba kodą), kad ištekliai nebūtų naudojami per daug.</span><span class="sxs-lookup"><span data-stu-id="efc94-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="efc94-110">Daugiau informacijos apie buferizavimo pamatyti, [išvengti gauti neleista arba užblokuotas SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="efc94-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="efc94-111">Jei naudodami **klasikinę** arba **modernią** "SharePoint" svetainę ar puslapį jaučiate lėto veikimo efektyvumą, pasinaudokite [puslapio diagnostikos įrankiu](https://aka.ms/perftool) puslapiams analizuoti.</span><span class="sxs-lookup"><span data-stu-id="efc94-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="efc94-112">Jei vis dar patirtis apskritai lėto veikimo, prašome peržiūrėti išteklius šio straipsnio apačioje: [Įvadas į veiklos reguliavimas SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="efc94-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  