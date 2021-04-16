---
title: Pirštų atspaudų atrakinimo parinkties naudojimas "Windows 10"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796685"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Pirštų atspaudų atrakinimo parinkties naudojimas "Windows 10"

**"Windows Hello" piršto atspaudo įgalinkite**

Norėdami atrakinti "Windows 10" naudodami piršto atspaudą, turite nustatyti "Windows Hello Fingerprint" įtraukdami (leisdami "Windows" išmokti atpažinti) bent vienu pirštu. 

1. Eikite **į Parametrai > Paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)). Bus išvardytos galimos prisijungimo parinktys. Toliau pateikiami pavyzdžiai.

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. Spustelėkite arba bakstelėkite **"Windows Hello Fingerprint"**, tada **spustelėkite Nustatyti**. Lange "Windows Hello" sąranka spustelėkite **Darbo pradžia**. Pirštų atspaudų jutiklis suaktyvins ir būsite paprašyti pirštu padėti ant jutiklio:

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. Vykdykite nurodymus, kuriuose bus nurodyta pakartotinai nuskaityti pirštą. Kai tai bus baigta, galėsite įtraukti kitų pirštų, kuriuos galbūt norėsite naudoti prisijungdami. Kai kitą kartą prisijungsite prie "Windows 10", turėsite galimybę naudoti pirštų atspaudą.

**"Windows Hello Fingerprint" nėra kaip prisijungimo parinktis**

Jei "Windows Hello Fingerprint" nėra rodoma kaip parinktis prisijungimo parinktyse, tai reiškia, kad "Windows" nežino apie pirštų atspaudų skaitytuvą / skaitytuvą, pridėtą prie jūsų kompiuterio, arba kad sistemos strategija neleidžia jo naudoti (pvz., jei jūsų kompiuterį valdo jūsų darbovietė). Norėdami šalinti triktis: 

1. Užduočių **juostoje pasirinkite** mygtuką Pradžia ir ieškokite Įrenginių **tvarkytuvė.**

2. Spustelėkite arba bakstelėkite, kad atidarytumėte **įrenginių tvarkytuvę.**

3. Įrenginių tvarkytuvėje išplėskite Biometriniai įrenginiai spustelėdami savo "v" pavidalo.

   ![Biometriniai įrenginiai.](media/biometric-devices.png)

4. Jūsų pirštų atspaudų skaitytuvas turi būti nurodytas kaip biometrinis įrenginys, pvz., "Synaptics WBDI" skaitytuvas:

   ![Biometriniai įrenginiai.](media/biometric-devices-expanded.png)

5. Jei pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į jūsų kompiuterį, eikite į kompiuterio gamintojo svetainę. Kompiuterio modelio techninio palaikymo skyriuje ieškokite skaitytuvo, kurį galite įdiegti, "Windows 10" tvarkyklės.

6. Jei skaitytuvas yra atskirtas nuo kompiuterio (pridėto per USB), eikite į skaitytuvo gamintojo svetainę, kad rastumėte ir įdiegtumėte "Windows 10" įrenginio tvarkyklės programinę įrangą, skirtą jūsų turimo skaitytuvo modeliui.
