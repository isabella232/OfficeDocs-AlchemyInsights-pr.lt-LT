---
title: "\"Apple\" automatinio įrenginio registracijos sinchronizavimo klaidos"
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013756"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>"Apple" automatinio įrenginio registracijos sinchronizavimo klaidos

"Aptikome, kad turite vieną ar daugiau ADE/DEP atpažinimo ženklų, kurių būsena yra klaida. Kol klaidos būsena nebus išspręsta kiekvienam paveiktam atpažinimo ženklui, ADE funkcija neveiks taip, kaip tikėtasi.".

Ši klaida gali būti rodoma keliais būdais, įskaitant:

1. Įrenginiai gali būti nesinchronizuojami iš ABM / ASM į "Intune"
2. Registracijos profilio užduotys gali nepavykti
3. Įrenginiai gali nepavykti sėkmingai užregistruoti ADE

Patikrinkite sinchronizavimo klaidą, apie kurią pranešta "Intune" konsolėje dalyje **Įrenginiai, > Registruoti įrenginius > "Apple" registracija > registracijos programos atpažinimo ženklus.**

Viena iš dažniausių sinchronizavimo klaidos priežasčių yra dabartinio atpažinimo ženklo galiojimo pabaiga. Daugeliu atvejų problema bus išspręsta atnaujinus paveiktą atpažinimo ženklą.

Jei baigėsi vieno ar daugiau atpažinimo ženklų galiojimo laikas, žr. toliau nurodytą dokumentaciją, kad prireikus juos atnaujintumėte:

[Automatinio įrenginio registracijos atpažinimo ženklo atnaujinimas](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Be to, galite matyti toliau nurodytą dokumentaciją, kad pamatytumėte galimas kitų klaidų, dėl kurių kyla atpažinimo ženklo sinchronizavimo klaidų, ištaisymą:

["iOS" / "iPadOS" ir "macOS" automatinių įrenginių registracijos atpažinimo ženklų ABM / ASM sinchronizavimo klaidos](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







["iOS" / "iPadOS" ir "macOS" automatinių įrenginių registracijos atpažinimo ženklų ABM / ASM sinchronizavimo klaidos](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
