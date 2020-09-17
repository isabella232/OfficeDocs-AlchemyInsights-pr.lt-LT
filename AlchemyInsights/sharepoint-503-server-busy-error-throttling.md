---
title: "\"SharePoint Online\" buferizavimo"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773855"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5bd48-102">"SharePoint Online" buferizavimo</span><span class="sxs-lookup"><span data-stu-id="5bd48-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5bd48-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="5bd48-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5bd48-104">**"503" serveris užimtas**</span><span class="sxs-lookup"><span data-stu-id="5bd48-104">**503 server is busy error**</span></span>

<span data-ttu-id="5bd48-105">Vartotojai gali gauti "503" serveris yra užimtas klaida bandant pereiti į "SharePoint" arba "OneDrive" svetaines.</span><span class="sxs-lookup"><span data-stu-id="5bd48-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5bd48-106">Šią klaidą gali sukelti "SharePoint" tarnyboje.</span><span class="sxs-lookup"><span data-stu-id="5bd48-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5bd48-107">„SharePoint Online“ naudoja ribojimo funkciją, kad užtikrintų optimalų „SharePoint Online“ paslaugos veiksmingumą ir patikimumą.</span><span class="sxs-lookup"><span data-stu-id="5bd48-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5bd48-108">Ribojimas apriboja vartotojo veiksmų arba vienu metu vykstančių skambučių (pagal scenarijų ar kodą) skaičių, kad būtų užkirstas kelias per dideliam išteklių naudojimui.</span><span class="sxs-lookup"><span data-stu-id="5bd48-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="5bd48-109">Daugiau informacijos apie buferizavimą rasite " [SharePoint Online" negauti ribojimo arba užblokuotas](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5bd48-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5bd48-110">Jei manote, kad ši klaida yra nesusijusi su buferizacija, galite patikrinti, ar jūsų nuomotojuje yra aktyvi priežiūra, kai naršote [pranešimų centre](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="5bd48-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5bd48-111">Galiausiai, įsitikinkite, kad apsilankysite [tarnybos sveikatos](https://portal.office.com/adminportal/home#/servicehealth) puslapyje, kad patikrintumėte, ar yra kokių nors galinčių įvykti incidentų.</span><span class="sxs-lookup"><span data-stu-id="5bd48-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

