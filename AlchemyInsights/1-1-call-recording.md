---
title: 1:1 skambučių įrašymas
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733857"
---
# <a name="11-call-recording"></a>1:1 skambučių įrašymas

Administratoriai turi imtis veiksmų dabar, kad vartotojai galėtų įrašyti "1:1" iškvietimus.
 
Pradėję balandžio 12 d., 2021, pradėsime vykdyti naują komandų skambinimo strategijos parinktį *Allowcloudrecordingforcalls*. 

Šiuo metu "1:1" skambučių įrašymo galimybes kontroliuoja "teams" susitikimo strategijų parinktis *Allowcloudrecording* . Jei vartotojams leidžiama įrašyti komandų susitikimus, jie taip pat gali įrašyti "1:1" skambutį.

Jei norite blokuoti visus vartotojus, kad įrašytumėte "1:1" iškvietimus, jums nereikia imtis jokių veiksmų. Numatytoji parinktis *Allowcloudrecordingforcalls* skambinimo strategija bus $FALSE.

Šis pakeitimas dokumentuojamas šiame pranešimų centro pranešime: [(atnaujinta) "1:1" skambučių įrašymo strategijos Įvadas](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Norėdami nustatyti "teams" skambinimo strategijos parinktį, turite naudoti " [teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)".

**Skambučio įrašymo įgalinimas "1:1" pokalbiuose:** Set-CsTeamsCallingPolicy – tapatybė visuotinis – AllowCloudRecordingForCalls $TRUE

**Norėdami išjungti skambučio įrašymą "1:1" pokalbiuose:** Set-CsTeamsCallingPolicy – tapatybė visuotinis – AllowCloudRecordingForCalls $FALSE

