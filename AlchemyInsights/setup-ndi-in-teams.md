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
# <a name="turn-on-ndi-technology"></a>NDI technologijos įjungimas

NDI technologija reikalauja dviejų veiksmų, kurie turi būti įjungti vartotojui:

1. Nuomotojo administratorius turi įgalinti "AllowNDIStreaming" ypatybę "Csteamstikos Meetingpolicy".

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Atlikus šį keitimą, galutinis vartotojas turi įjungti NDI® technologiją konkrečiam klientui iš **parametrų > teisės**.

Daugiau informacijos ieškokite [NDI technologijos naudojimas "Microsoft teams"](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
