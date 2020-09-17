---
title: Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795252"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"

**"Windows Hello" piršto atspaudo įgalinimas**

Jei norite atrakinti "Windows 10" naudodami pirštų atspaudus, turite nustatyti "Windows Hello" pirštų atspaudus, įtraukdami ("Windows" išmokę atpažinti) bent vieną pirštą. 

1. Eikite į **parametrai > paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)). Bus įtrauktos galimos prisijungimo parinktys. Pavyzdžiui:

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. Spustelėkite arba bakstelėkite **"Windows Hello" piršto atspaudas**, tada spustelėkite **nustatyti**. "Windows Hello" sąrankos **lange spustelėkite pradėti**. Pirštų atspaudų jutiklis suaktyvinamas ir būsite paraginti įdėti pirštą ant jutiklio:

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. Vykdykite nurodymus, kurie paprašys pakartotinai nuskaityti pirštą. Kai tai bus baigta, turėsite galimybę įtraukti kitų pirštų, kuriuos galbūt norėsite naudoti prisijungdami. Kai prisijungsite prie "Windows 10", turėsite galimybę naudoti pirštų atspaudus.

**"Windows Hello" piršto atspaudas negalimas kaip prisijungimo parinktis**

Jei "Windows Hello" kontrolinis kodas nerodomas kaip parinktis **prisijungimo parinktyse**, vadinasi, "Windows" nežino apie bet kokį pirštų atspaudų skaitytuvą/skaitytuvą, prijungtą prie jūsų kompiuterio, arba kad sistemos strategija neleidžia jos naudoti (pvz., jūsų kompiuterį tvarko jūsų darbo vieta). Norėdami pašalinti triktis: 

1. Pasirinkite mygtuką **Pradžia** užduočių juostoje ir ieškokite **įrenginių tvarkytuvė**.

2. Spustelėkite arba bakstelėkite, kad atidarytumėte **įrenginių tvarkytuvę**.

3. Įrenginių tvarkytuvėje išplėskite biometrinius įrenginius spustelėdami jo ševroną.

   ![Biometriniai įrenginiai.](media/biometric-devices.png)

4. Jūsų pirštų atspaudų skaitytuvas turi būti pateiktas kaip biometrinis įrenginys, pvz., "Synaptics WBDI" skaitytuvas:

   ![Biometriniai įrenginiai.](media/biometric-devices-expanded.png)

5. Jei jūsų pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į jūsų kompiuterį, eikite į kompiuterio gamintojo svetainę. KOMPIUTERIO modelio techninio palaikymo sekcijoje ieškokite "Windows 10" tvarkyklės, skirtos skaitytuvui, kurį galite įdiegti.

6. Jei skaitytuvas yra atskirtas nuo asmeninio kompiuterio (pridėto per USB), eikite į skaitytuvo gamintojo svetainę ir raskite bei įdiekite "Windows 10" įrenginio tvarkyklės programinę įrangą, skirtą skaitytuvo modeliui.
