---
title: "\"Windows\" atminties diagnostikos paleidimas sistemoje \"Windows 10\""
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826675"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>"Windows" atminties diagnostikos paleidimas sistemoje "Windows 10"

Jei "Windows" ir kompiuterio programėlės sugenda, užstringa arba veikia nestabiliai, gali kilti kompiuterio atminties (RAM) problemų. Galite paleisti "Windows" atminties diagnostiką, kad patikrinsite kompiuterio RAM problemas.

Užduočių juostos ieškos lauke įveskite atminties **diagnostika**, tada pasirinkite **"Windows" atminties diagnostika**. 

Norėdami vykdyti diagnostiką, kompiuteris turi būti paleistas iš naujo. Turite galimybę iš naujo paleisti iš karto (pirmiausia įrašykite savo darbą ir uždarykite atidarytus dokumentus ir el. laiškus) arba suplanuoti diagnostiką, kad ji būtų vykdoma automatiškai, kai kompiuteris bus paleistas iš naujo:

!["Windows" atminties diagnostika](media/windows-memory-diagnostic.png)

Kai kompiuteris bus paleistas iš naujo, **"Windows" atminties diagnostikos įrankis** bus paleistas automatiškai. Būsena ir eiga bus rodomi kaip diagnostika, o jūs turite galimybę atšaukti diagnostiką paspaudus **klaviatūros klavišą ESC.**

Kai diagnostika bus baigta, "Windows" pradės įprastai.
Iš karto po paleidimo iš naujo, kai rodomas  darbalaukis, bus rodomas pranešimas (užduočių juostoje šalia veiksmų centro piktogramos), nurodantis, ar rasta atminties klaidų. Toliau pateikiami pavyzdžiai.

Štai veiksmų centro piktograma: ![Veiksmų centro piktograma](media/action-center-icon.png) 

Ir pranešimo pavyzdys: ![Nėra atminties klaidų](media/no-memory-errors.png)

Jei praleidote pranešimą, užduočių juostoje galite pasirinkti veiksmų centro piktogramą, kad būtų rodomas veiksmų **centras** ir rodomas slenkamas pranešimų sąrašas. 

Norėdami peržiūrėti išsamią informaciją, **įveskite įvykį** užduočių juostos ieškos lauke, tada pasirinkite Įvykių **peržiūros programa**. Įvykių **peržiūros programos kairiojoje** srityje eikite į **"Windows" žurnalai > Sistema**. Dešiniosios srities srityje nuskaitykite sąrašą žiūrėdami į stulpelį Šaltinis, kol pamatysite įvykius su šaltinio reikšme **MemoryDiagnostics-Results**.  Pažymėkite kiekvieną tokį įvykį ir peržiūrėkite rezultato informaciją lauke **po skirtuku Bendra** po sąrašu.
