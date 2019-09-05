---
title: "\"SharePoint Online\" užklausų Buferėjimas"
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751896"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="6ea74-102">"SharePoint Online" užklausų Buferėjimas</span><span class="sxs-lookup"><span data-stu-id="6ea74-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="6ea74-103">Vartotojai gali gauti 503 serverio yra užimtas klaida bandant pereiti prie SharePoint arba OneDrive svetainių.</span><span class="sxs-lookup"><span data-stu-id="6ea74-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="6ea74-104">Ši klaida gali kilti dėl buferinės per SharePoint tarnybos.</span><span class="sxs-lookup"><span data-stu-id="6ea74-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6ea74-105">SharePoint Online naudoja buferizavimo išlaikyti optimalų efektyvumą ir patikimumą SharePoint Online paslaugos.</span><span class="sxs-lookup"><span data-stu-id="6ea74-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6ea74-106">Buferinis ribojimas riboja vartotojo veiksmų arba vienu metu vykstančių skambučių skaičių (pagal scenarijų arba kodą), kad ištekliai nebūtų naudojami per daug.</span><span class="sxs-lookup"><span data-stu-id="6ea74-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="6ea74-107">Jei jūs gaunate Throttled, 99% laiko tai dėl pasirinktinį kodą.</span><span class="sxs-lookup"><span data-stu-id="6ea74-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="6ea74-108">Daugiau informacijos apie buferizavimo pamatyti, [išvengti gauti neleista arba užblokuotas SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="6ea74-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="6ea74-109">Jei manote, kad ši klaida yra nesusijusi su užklausų buferiu, galite patikrinti, ar jūsų nuomininkui yra aktyvi priežiūra, pereidami į [pranešimų centrą](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="6ea74-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="6ea74-110">Galiausiai, įsitikinkite, kad lankotės [tarnybos sveikatos](https://portal.office.com/adminportal/home#/servicehealth) puslapyje patikrinti, ar nėra patarimų/incidentų, kurie gali būti vyksta.</span><span class="sxs-lookup"><span data-stu-id="6ea74-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

