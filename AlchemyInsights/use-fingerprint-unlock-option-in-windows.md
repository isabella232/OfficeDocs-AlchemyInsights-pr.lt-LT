---
title: Pirštų atspaudų atrakinimo parinkties naudojimas Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971943"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Pirštų atspaudų atrakinimo parinkties naudojimas Windows 10

**Įgalinti Windows Hello piršto atspaudą**

Norėdami atrakinti Windows 10 piršto atspaudą, turite nustatyti pirštų Windows Hello įtraukdami (Windows išmokti atpažinti) bent vieną pirštą. 

1. Eikite **į Parametrai > Paskyros > prisijungimo parinktis** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)). Bus išvardytos galimos prisijungimo parinktys. Toliau pateikiami pavyzdžiai.

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. Spustelėkite arba bakstelėkite **Windows Hello piršto atspaudą**, **tada spustelėkite Nustatyti**. Lange Windows Hello spustelėkite **Darbo pradžia**. Pirštų atspaudų jutiklis suaktyvins ir būsite paprašyti pirštu padėti ant jutiklio:

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. Vykdykite nurodymus, kuriuose bus nurodyta pakartotinai nuskaityti pirštą. Kai tai bus baigta, galėsite įtraukti kitų pirštų, kuriuos galbūt norėsite naudoti prisijungdami. Kai kitą kartą prisijungsite prie Windows 10, turėsite galimybę naudoti piršto atspaudą.

**Windows Hello Piršto atspaudas negalimas kaip prisijungimo parinktis**

Jei "Windows Hello" piršto atspaudas nerodomas kaip parinktis prisijungimo parinktyse, tai reiškia, kad "Windows" nežino jokių prie jūsų kompiuterio pridėtų pirštų atspaudų skaitytuvo / skaitytuvo arba kad sistemos strategija neleidžia jo naudoti (pvz., jei jūsų kompiuterį valdo jūsų darbovietė). Norėdami šalinti triktis: 

1. Užduočių **juostoje pasirinkite** mygtuką Pradžia ir ieškokite Įrenginių **tvarkytuvė.**

2. Spustelėkite arba bakstelėkite, kad atidarytumėte **įrenginių tvarkytuvę.**

3. Įrenginių tvarkytuvėje išplėskite Biometriniai įrenginiai spustelėdami savo "v" pavidalo.

   ![Biometriniai įrenginiai.](media/biometric-devices.png)

4. Jūsų pirštų atspaudų skaitytuvas turi būti nurodytas kaip biometrinis įrenginys, pvz., "Synaptics WBDI" skaitytuvas:

   ![Biometriniai įrenginiai.](media/biometric-devices-expanded.png)

5. Jei pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į jūsų kompiuterį, eikite į kompiuterio gamintojo svetainę. Kompiuterio modelio techninio palaikymo skyriuje ieškokite Windows 10 skaitytuvo, kurį galite įdiegti, tvarkyklės.

6. Jei skaitytuvas yra atskirtas nuo kompiuterio (pridėto per USB), eikite į skaitytuvo gamintojo svetainę, kad rastumėte ir įdiegtumėte Windows 10 įrenginio tvarkyklės programinę įrangą jūsų turimo skaitytuvo modeliui.
