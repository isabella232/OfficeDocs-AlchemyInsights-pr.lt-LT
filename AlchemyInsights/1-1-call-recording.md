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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314392"
---
# <a name="11-call-recording"></a>1:1 skambučio įrašymas

Jei mygtukas **Pradėti** įrašymą yra pilkas 1:1 skambučio metu, turite pakeisti paveikto vartotojo strategijos parametrus. Norėdami patikrinti strategijos parametrą, paleiskite paveikto vartotojo diagnostiką **įvesdami Diag: Teams 1:1 Call Recording** above.     

Nuo 2021 m. gegužės 31 d. pradėsime taikyti naują skambučių Teams *AllowCloudRecordingForCalls.* Prieš šį keitimą 1:1 skambučio įrašymą valdo *"AllowCloudRecording"* Teams susitikimo strategija. Šis pakeitimas dokumentuojamas pranešimų centro skelbime: [(atnaujinta) 1:1 Skambučių įrašymo strategijos įvadas](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   skambinimo strategijos parinktis nustatyta **kaip $False pagal** numatytuosius nustatymus. Jei norite blokuoti visus vartotojus nuo 1:1 skambučių įrašymo, jums nereikia atlikti jokių veiksmų.  

Norėdami įgalinti skambučių įrašymą visiems vartotojams 1:1 [skambučiuose, naudokite "Teams PowerShell",](https://docs.microsoft.com/microsoftteams/teams-powershell-install) kad paleistumėte šią "cmdlet": 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Taip pat galite sukurti naują strategiją ir **nustatyti -AllowCloudRecordingForCalls** **$true** priskirti šią strategiją savo vartotojams. 

Daugiau informacijos žr. [1:1 Skambučių įrašymo strategijos valdikliai yra (beveik!) Čia](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
