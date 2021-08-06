---
title: Paleisti Windows atminties diagnostiką Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922579"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Paleisti Windows atminties diagnostiką Windows 10

Jei Windows kompiuterio programėlės sugenda, užšaldomos arba veikia nestabiliai, gali kilti kompiuterio atminties (RAM) problemų. Galite paleisti "Windows diagnostiką, kad patikrinsite, ar nėra kompiuterio RAM problemų.

Užduočių juostos ieškos lauke įveskite atminties **diagnostika**, tada pasirinkite Windows **diagnostika**. 

Norėdami vykdyti diagnostiką, kompiuteris turi būti paleistas iš naujo. Turite galimybę iš naujo paleisti iš karto (pirmiausia įrašykite savo darbą ir uždarykite atidarytus dokumentus ir el. laiškus) arba suplanuoti diagnostiką, kad ji būtų vykdoma automatiškai, kai kompiuteris bus paleistas iš naujo:

![Windows Atminties diagnostika](media/windows-memory-diagnostic.png)

Kai kompiuteris paleidžiamas iš naujo, **Windows atminties diagnostikos įrankis** bus paleistas automatiškai. Būsena ir eiga bus rodomi kaip diagnostika, o jūs turite galimybę atšaukti diagnostiką paspaudus **klaviatūros klavišą ESC.**

Kai diagnostika bus baigta, Windows bus pradėti įprastai.
Iš karto po paleidimo iš naujo, kai rodomas  darbalaukis, bus rodomas pranešimas (užduočių juostoje šalia veiksmų centro piktogramos), nurodantis, ar rasta atminties klaidų. Toliau pateikiami pavyzdžiai.

Štai veiksmų centro piktograma: ![Veiksmų centro piktograma](media/action-center-icon.png) 

Ir pranešimo pavyzdys: ![Nėra atminties klaidų](media/no-memory-errors.png)

Jei praleidote pranešimą, užduočių juostoje galite pasirinkti veiksmų centro piktogramą, kad būtų rodomas veiksmų **centras** ir rodomas slenkamas pranešimų sąrašas. 

Norėdami peržiūrėti išsamią informaciją, **įveskite įvykį** užduočių juostos ieškos lauke, tada pasirinkite Įvykių **peržiūros programa**. Įvykių **peržiūros programos** kairiojoje srityje eikite į Windows **Žurnalai > sistema**. Dešiniosios srities srityje nuskaitykite sąrašą žiūrėdami į stulpelį Šaltinis, kol pamatysite įvykius su šaltinio reikšme **MemoryDiagnostics-Results**.  Pažymėkite kiekvieną tokį įvykį ir peržiūrėkite rezultato informaciją lauke **po skirtuku Bendra** po sąrašu.
