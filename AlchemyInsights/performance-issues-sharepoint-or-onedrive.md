---
title: Efektyvumo problemos – "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771909"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="21bcf-102">"SharePoint" arba "OneDrive" lėtas, nepasiekiamas arba nepasiekiamas keliems vartotojams</span><span class="sxs-lookup"><span data-stu-id="21bcf-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="21bcf-103">"SharePoint" arba "OneDrive" gali būti lėta, neprieinama arba neprieinama arba gali būti rodoma paslauga neprieinama arba 503 klaidos dėl kelių priežasčių:</span><span class="sxs-lookup"><span data-stu-id="21bcf-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="21bcf-104">Jei jūsų "SharePoint" arba "OneDrive" svetainė yra lėta ar atidėta keliems vartotojams, gali būti laikina tarnybos problema, dėl kurios vartotojai susiduria su pertrūkiais arba naršymo klaidomis, kai jungiasi prie "SharePoint" svetainių arba "OneDrive" turinio.</span><span class="sxs-lookup"><span data-stu-id="21bcf-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="21bcf-105">Patikrinkite [tarnybos sveikatos ataskaitų sritį](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ir Sužinokite, ar jūsų organizacija turi įtakos.</span><span class="sxs-lookup"><span data-stu-id="21bcf-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="21bcf-106">Vartotojai gali gauti " *503" serveris yra užimtas* klaida bandant pereiti į "SharePoint" arba "OneDrive" svetaines.</span><span class="sxs-lookup"><span data-stu-id="21bcf-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="21bcf-107">Šią klaidą gali sukelti "SharePoint" tarnyboje.</span><span class="sxs-lookup"><span data-stu-id="21bcf-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="21bcf-108">„SharePoint Online“ naudoja ribojimo funkciją, kad užtikrintų optimalų „SharePoint Online“ paslaugos veiksmingumą ir patikimumą.</span><span class="sxs-lookup"><span data-stu-id="21bcf-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="21bcf-109">Ribojimas apriboja vartotojo veiksmų arba vienu metu vykstančių skambučių (pagal scenarijų ar kodą) skaičių, kad būtų užkirstas kelias per dideliam išteklių naudojimui.</span><span class="sxs-lookup"><span data-stu-id="21bcf-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="21bcf-110">Daugiau informacijos apie buferizavimą rasite " [SharePoint Online" negauti ribojimo arba užblokuotas](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="21bcf-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="21bcf-111">Jei su **klasikine** arba **šiuolaikine** "SharePoint" svetaine ar puslapiu susiduriate lėčiau, naudokite [puslapį diagnostikos įrankis](https://aka.ms/perftool) , kad išanalizuotumėte puslapius.</span><span class="sxs-lookup"><span data-stu-id="21bcf-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="21bcf-112">Jei vis dar susiduriate su bendrąja lėtu veikimu, peržiūrėkite išteklius šio straipsnio apačioje: [Įvadas į "SharePoint Online" našumo reguliavimą](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="21bcf-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  