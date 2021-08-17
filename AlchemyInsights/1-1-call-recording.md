---
title: 1:1 skambučio įrašymas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886147"
---
# <a name="11-call-recording"></a>1:1 skambučio įrašymas

Jei mygtukas **Pradėti** įrašymą yra pilkas 1:1 skambučio metu, turite pakeisti paveikto vartotojo strategijos parametrus. Norėdami patikrinti strategijos parametrą, paleiskite paveikto vartotojo diagnostiką įvesdami **Diag: Teams 1:1 Call Recording** above.     

Nuo 2021 m. gegužės 31 d. pradėsime taikyti naują skambučių Teams *AllowCloudRecordingForCalls.* Prieš šį keitimą 1:1 skambučio įrašymas valdomas *"AllowCloudRecording"* Teams susitikimo strategijos. Šis pakeitimas dokumentuojamas pranešimų centro skelbime: [(atnaujinta) 1:1 Skambučių įrašymo strategijos įvadas](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   skambinimo strategijos parinktis nustatyta **kaip $False pagal** numatytuosius parametrus. Jei norite blokuoti visus vartotojus nuo 1:1 skambučių įrašymo, jums nereikia atlikti jokių veiksmų.  

Norėdami įgalinti skambučių įrašymą visiems vartotojams 1:1 skambučiuose, [naudokite "Teams PowerShell",](https://docs.microsoft.com/microsoftteams/teams-powershell-install) kad paleistumėte šią "cmdlet": 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Taip pat galite sukurti naują strategiją ir **nustatyti -AllowCloudRecordingForCalls** **$true** priskirti šią strategiją vartotojams. 

Daugiau informacijos žr. [1:1 Skambučių įrašymo strategijos valdikliai yra (beveik!) Čia](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
