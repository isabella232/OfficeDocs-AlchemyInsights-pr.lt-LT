---
title: "\"TeamViewer\" naudojimas nuotoliniu būdu administruoti \"Intune\" įrenginius"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555242"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>"TeamViewer" naudojimas nuotoliniu būdu administruoti "Intune" įrenginius

"Intune" valdomi įrenginiai gali būti administruojami nuotoliniu būdu naudojant ["TeamViewer".](https://www.teamviewer.com/)

Norėdami administruoti "Intune" naudodami "TeamViewer", atlikite šiuos veiksmus: 

Pradėkite gaudami kredencialus iš "TeamViewer", kad nustatytumėte "TeamViewer Connector" intune. Tai leidžia administratoriui įvesti kredencialus "TeamViewer Connector" vartotojo sąsajoje įrenginiai, vienkartinė operacija, siekiant nustatyti ryšį tarp "Intune" ir "TeamViewer" paslaugos.

**1 dalis: pradėkite seansą naudodami nuotolinį įrenginį**

1. Dalyje **Visi įrenginiai**pasirinkite įrenginį, su kuriuo norite pradėti nuotolinį seansą.
2. Nuo **... Daugiau**, pasirinkite **Naujas nuotolinės pagalbos seansas**.
3. Pasirinkite **Taip,** kad patvirtintumėte, jog norite nustatyti nuotolinį seansą.
    "TeamViewer" tarnybai patvirtinus užklausą "Pradėti naują nuotolinį seansą", įrenginio apžvalgos (arba "Essentials") srityje matysite parinktį **Pradėti nuotolinę pagalbą.** Pasirinkite **Žiūrėti daugiau,** kad išplėstumėte sritį ir parodytumėte nuotolinės pagalbos būseną.
4. Pasirinkite **Pradėti nuotolinį seansą,** kad inicijuotumėte seansą administratoriaus pusėje.
5. Pasirinkite atsisiųsti "TeamViewer" dvejetainį ("Windows") ir pasirinkite **Vykdyti**.<br/>
    **Pastaba** Galite nepaisyti bet kurio žiniatinklio naršyklės puslapio, atidaryto "TeamViewer" svetainėje.

6. Patvirtinkite "TeamViewer" programėlės prašymą atlikti pakeitimus įrenginyje (tik "Windows").
7. Paleidžiama "TeamViewer" programa, į kurią įtraukiamas seanso kodas, skirtas ryšio su nuotoliniu įrenginiu autentifikuoti.

**2 dalis: Įrenginyje, skirtame nuotoliniam seansui**

1. Atidarykite įmonės portalą Intune.
2. Ieškokite pranešimo vėliavėlės: "Jūsų IT administratorius prašo valdyti šį įrenginį nuotolinės pagalbos seansui", ir pasirinkite pranešimą.
3. Pasirinkite atsisiųsti "TeamViewer" programą arba patvirtinti "TeamViewer" programos atsisiuntimą iš programų parduotuvės ir pasirinkite **Vykdyti**.
    **Pastaba** Galite nepaisyti bet kurio žiniatinklio naršyklės puslapio, atidaryto "TeamViewer" svetainėje.

4. Patvirtinkite "TeamViewer" programėlės prašymą atlikti pakeitimus įrenginyje (tik "Windows").
5. Paleidžiama "TeamViewer" programa, į kurią įtraukiamas seanso kodas, skirtas ryšio su nuotoliniu įrenginiu autentifikuoti.
6. Iššokantis langas klausia, ar norite leisti pradėti seansą.

**Pastaba** "TeamViewer" tarnybos sugeneruoti seanso kodai naudojami tik vieną kartą. Jei prarasite ryšį, turite:

1. Uždarykite "TeamViewer" programos egzempliorių nuotoliniame įrenginyje ir administratoriaus darbo vietoje.
2. Uždarykite nuotolinio įrenginio įmonės portalą.
3. Inicijuoti naują "Naują nuotolinės pagalbos seansą" iš administravimo portalo.
4. Iš naujo atidarykite nuotolinio įrenginio įmonės portalą, kad gautumėte naują pranešimą.
5. Atsisiųskite ir atidarykite "TeamViewer" programą nuotoliniame įrenginyje ir administratoriaus darbo vietoje, kaip ir anksčiau.