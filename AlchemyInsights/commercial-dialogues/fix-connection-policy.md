---
title: Ryšio strategijos taisymas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314852"
---
# <a name="fix-connection-policy"></a>Ryšio strategijos taisymas

El. laiškas buvo pažymėtas saugus ir pristatytas į vartotojo aplanką Gauta, nes šaltinio IP adresas buvo pažymėtas kaip saugus pagal numatytąją ryšio filtro strategiją. Norėdami peržiūrėti strategiją, atlikite šiuos veiksmus:

1. ""Microsoft 365" sargyba" portale eikite į El. & bendradarbiavimo <https://security.microsoft.com/> strategijos &  \> **Taisyklės** \> **Grėsmių** \>   strategijos Apsauga nuo pašto šiukšlių skyriuje Strategijos.

   Norėdami pereiti tiesiai į apsaugos **nuo pašto šiukšlių strategijų** puslapį, naudokite <https://security.microsoft.com/antispam> .

2. Puslapyje **Apsaugos nuo pašto šiukšlių** strategijos pasirinkite strategiją, pavadintą Ryšio filtro strategija **(numatytoji),** spustelėdami strategijos pavadinimą.

3. Rodomame išsamios informacijos iškeliamyje spustelėkite **Redaguoti ryšio filtro strategiją** dalyje Ryšio **filtravimas.**

4. Peržiūrėkite įrašus **sekcijoje Visada leisti pranešimus** iš šių IP adresų arba adresų diapazono ir sužinokite, **ar pasirinkta Įjungti saugų** sąrašą.

   **Pastaba:**"Microsoft" prenumeruoja trečiųjų šalių patikimų siuntėjų šaltinius. Jei įgalintas saugus sąrašas, šie patikimi siuntėjai klaidingai nepažymimi kaip pašto šiukšlės. Rekomenduojame pasirinkti šią parinktį, nes ji sumažins gautų klaidingai teigiamų laiškų (gerų laiškų, kurie klasifikuojami kaip pašto šiukšlės) skaičių.

Daugiau informacijos žr. [Ryšio filtravimo konfigūravimas](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
