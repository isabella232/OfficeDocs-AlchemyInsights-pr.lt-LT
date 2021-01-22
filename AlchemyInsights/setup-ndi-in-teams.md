---
title: NDI technologijos įjungimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935132"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="2dbb9-102">NDI technologijos įjungimas</span><span class="sxs-lookup"><span data-stu-id="2dbb9-102">Turn on NDI technology</span></span>

<span data-ttu-id="2dbb9-103">NDI technologija reikalauja dviejų veiksmų, kurie turi būti įjungti vartotojui:</span><span class="sxs-lookup"><span data-stu-id="2dbb9-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="2dbb9-104">Nuomotojo administratorius turi įgalinti "AllowNDIStreaming" ypatybę "Csteamstikos Meetingpolicy".</span><span class="sxs-lookup"><span data-stu-id="2dbb9-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="2dbb9-105">Atlikus šį keitimą, galutinis vartotojas turi įjungti NDI® technologiją konkrečiam klientui iš **parametrų > teisės**.</span><span class="sxs-lookup"><span data-stu-id="2dbb9-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="2dbb9-106">Daugiau informacijos ieškokite [NDI technologijos naudojimas "Microsoft teams"](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="2dbb9-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
