---
title: "\"SharePoint Online\" užklausų buferizavimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742217"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="321d3-102">"SharePoint Online" užklausų buferizavimas</span><span class="sxs-lookup"><span data-stu-id="321d3-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="321d3-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="321d3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="321d3-104">**503 serveris užimtas klaida**</span><span class="sxs-lookup"><span data-stu-id="321d3-104">**503 server is busy error**</span></span>

<span data-ttu-id="321d3-105">Vartotojai gali gauti 503 serveris yra užimtas klaida bandant pereiti į SharePoint "arba" OneDrive svetainėse.</span><span class="sxs-lookup"><span data-stu-id="321d3-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="321d3-106">Šią klaidą gali sukelti buferizavimas SharePoint tarnyboje.</span><span class="sxs-lookup"><span data-stu-id="321d3-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="321d3-107">„SharePoint Online“ naudoja ribojimo funkciją, kad užtikrintų optimalų „SharePoint Online“ paslaugos veiksmingumą ir patikimumą.</span><span class="sxs-lookup"><span data-stu-id="321d3-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="321d3-108">Ribojimas apriboja vartotojo veiksmų arba vienu metu vykstančių skambučių (pagal scenarijų ar kodą) skaičių, kad būtų užkirstas kelias per dideliam išteklių naudojimui.</span><span class="sxs-lookup"><span data-stu-id="321d3-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="321d3-109">Jei norite gauti daugiau informacijos apie buferizavimas [pamatyti, Išvengti gauti throttled arba užblokuotas SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="321d3-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="321d3-110">Jei manote, kad ši klaida nėra susijusi su buferizavimas, galite patikrinti, ar yra aktyvi priežiūra vyksta jūsų nuomotojo keliaudami į [pranešimų centrą](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="321d3-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="321d3-111">Galiausiai įsitikinkite, kad lankotės [puslapyje Tarnybos sveikata](https://portal.office.com/adminportal/home#/servicehealth) ir patikrinkite, ar nėra patarimų / incidentų, kurie gali įvykti.</span><span class="sxs-lookup"><span data-stu-id="321d3-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

