---
title: "\"SharePoint Online\" užklausų Buferėjimas"
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: ed3598dc92a7c36c9c9b077db0ab31f63537ef60
ms.sourcegitcommit: 14894a09db1c4101e48ff720d878d1c9f7b1dac8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/16/2019
ms.locfileid: "40065566"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="93015-102">"SharePoint Online" užklausų Buferėjimas</span><span class="sxs-lookup"><span data-stu-id="93015-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="93015-103">Vartotojai gali gauti 503 serverio yra užimtas klaida bandant pereiti prie SharePoint arba OneDrive svetainių.</span><span class="sxs-lookup"><span data-stu-id="93015-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="93015-104">Ši klaida gali kilti dėl buferinės per SharePoint tarnybos.</span><span class="sxs-lookup"><span data-stu-id="93015-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="93015-105">SharePoint Online naudoja buferizavimo išlaikyti optimalų efektyvumą ir patikimumą SharePoint Online paslaugos.</span><span class="sxs-lookup"><span data-stu-id="93015-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="93015-106">Buferinis ribojimas riboja vartotojo veiksmų arba vienu metu vykstančių skambučių skaičių (pagal scenarijų arba kodą), kad ištekliai nebūtų naudojami per daug.</span><span class="sxs-lookup"><span data-stu-id="93015-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="93015-107">Daugiau informacijos apie buferizavimo pamatyti, [išvengti gauti neleista arba užblokuotas SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="93015-107">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="93015-108">Jei manote, kad ši klaida yra nesusijusi su užklausų buferiu, galite patikrinti, ar jūsų nuomininkui yra aktyvi priežiūra, pereidami į [pranešimų centrą](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="93015-108">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="93015-109">Galiausiai, įsitikinkite, kad lankotės [tarnybos sveikatos](https://portal.office.com/adminportal/home#/servicehealth) puslapyje patikrinti, ar nėra patarimų/incidentų, kurie gali būti vyksta.</span><span class="sxs-lookup"><span data-stu-id="93015-109">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

