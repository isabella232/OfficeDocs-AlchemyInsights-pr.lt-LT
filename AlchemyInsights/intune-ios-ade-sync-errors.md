---
title: "\"Apple\" automatinio įrenginio registracijos Sinchronizavimo klaidos"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448930"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>"Apple" automatinio įrenginio registracijos Sinchronizavimo klaidos

"Nustatėme, kad turite vieną ar daugiau ad/DEP žetonų, kurie yra klaidos būsenos. Tol, kol bus išspręsta kiekvieno paveikto atpažinimo ženklo klaidos būsena, funkcija Ada neveiks taip, kaip tikėtasi. ".

Ši klaida gali pasireikšti įvairiais būdais, įskaitant:

1. Įrenginių negalima sinchronizuoti iš ABM/ASM į Intune
2. Registracijos profilio priskyrimai gali būti nepavykę
3. Įrenginiai gali sėkmingai neužbaigti ADE įtraukimo

Patikrinkite, ar sinchronizavimo klaida, pateikta "Intune" konsolėje, dalyje **įrenginiai > registruotis įrenginiai > "Apple" registracija > registracijos programos atpažinimo ženklai**.

Viena dažniausių Sinchronizavimo klaidos priežasčių yra dabartinio atpažinimo ženklo galiojimo laikas. Daugeliu atvejų paveikto atpažinimo ženklo atnaujinimas padės išspręsti problemą.

Jei vieno arba kelių jūsų žetonų galiojimas baigėsi, peržiūrėkite toliau pateiktus dokumentus, kad galėtumėte juos atnaujinti:

[Automatinio įrenginio registracijos atpažinimo ženklo atnaujinimas](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Be to, galite matyti toliau pateiktus dokumentus, kad matytumėte galimus kitų klaidų, sukėlusio simbolinės sinchronizavimo triktis, taisymus:

[ABM/ASM Sinchronizavimo klaidos, skirtos "iOS"/iPadOS ir "macOS" Automatizuotiems įrenginio registracijos žetonams](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM Sinchronizavimo klaidos, skirtos "iOS"/iPadOS ir "macOS" Automatizuotiems įrenginio registracijos žetonams](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
