---
title: Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588323"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"

**Įgalinti "Windows Hello" piršto atspaudą**

Norėdami atrakinti "Windows 10" naudodami piršto atspaudą, turite nustatyti "Windows Hello" pirštų atspaudą pridėdami (leisdami "Windows išmokti atpažinti") bent vienu pirštu. 

1. Eikite į **Parametrai > Paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)). Bus išvardytos galimos prisijungimo parinktys. Pavyzdžiui:

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. Spustelėkite arba bakstelėkite **"Windows Hello" pirštų atspaudas**, tada spustelėkite **Nustatyti**. "Windows Hello" sąrankos lange spustelėkite **Pradėti**. Pirštų atspaudų jutiklis įsijungs, o jūsų bus paprašyta pirštu padėti ant jutiklio:

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. Vykdykite nurodymus, kurie paprašys pakartotinai nuskaityti pirštą. Kai tai bus baigta, turėsite galimybę pridėti kitus pirštus, kuriuos galbūt norėsite naudoti prisijungdami. Kai kitą kartą prisijungsite prie "Windows 10", turėsite galimybę naudoti piršto atspaudą.

**"Windows Hello" pirštų atspaudų negalima kaip prisijungimo parinktis**

Jei **prisijungimo parinktyse**"Windows Hello" pirštų atspaudų nėra rodoma kaip parinktis, tai reiškia, kad "Windows" nežino jokio prie kompiuterio prijungto pirštų atspaudų skaitytuvo / skaitytuvo arba kad sistemos strategija neleidžia jo naudoti (pvz., jūsų kompiuterį valdo jūsų darbo vieta). Norėdami pašalinti: 

1. Užduočių **** juostoje pasirinkite pradžios mygtuką ir ieškokite **Įrenginių tvarkytuvės**.

2. Spustelėkite arba bakstelėkite , kad atidarytumėte **įrenginių tvarkytuvę**.

3. Įrenginių tvarkytuvėje išplėskite Biometriniai įrenginiai spustelėdami jo ševroną.

   ![Biometriniai prietaisai.](media/biometric-devices.png)

4. Pirštų atspaudų skaitytuvas turi būti nurodytas kaip biometrinis įrenginys, pvz., Synaptics WBDI skaitytuvas:

   ![Biometriniai prietaisai.](media/biometric-devices-expanded.png)

5. Jei pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į kompiuterį, eikite į kompiuterio gamintojo svetainę. Kompiuterio modelio techninio palaikymo skyriuje ieškokite skaitytuvo, kurį galite įdiegti, "Windows 10" tvarkyklės.

6. Jei skaitytuvas yra atskirtas nuo kompiuterio (prijungtas per USB), eikite į skaitytuvo gamintojo svetainę ir raskite ir įdiekite "Windows 10" įrenginio tvarkyklės programinę įrangą, skirtą jūsų skaitytuvo modeliui.
