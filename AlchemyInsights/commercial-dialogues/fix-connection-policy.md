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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888414"
---
# <a name="fix-connection-policy"></a>Ryšio strategijos taisymas

El. laiškas buvo pažymėtas saugus ir pristatytas į vartotojo aplanką Gauta, nes šaltinio IP adresas buvo pažymėtas kaip saugus pagal numatytąją ryšio filtro strategiją. Norėdami peržiūrėti strategiją, atlikite šiuos veiksmus:

1. ""Microsoft 365" sargyba" portale eikite į El. & bendradarbiavimo <https://security.microsoft.com/> strategijos &  \> **Taisyklės** \> **Grėsmių** \>   strategijos Apsauga nuo pašto šiukšlių skyriuje Strategijos.

   Norėdami pereiti tiesiai į apsaugos **nuo pašto šiukšlių strategijų** puslapį, naudokite <https://security.microsoft.com/antispam> .

2. Puslapyje **Apsaugos nuo pašto šiukšlių** strategijos pasirinkite strategiją, pavadintą Ryšio filtro strategija **(numatytoji),** spustelėdami strategijos pavadinimą.

3. Rodomame išsamios informacijos iškeliamyje spustelėkite **Redaguoti ryšio filtro strategiją** dalyje Ryšio **filtravimas.**

4. Peržiūrėkite įrašus **sekcijoje Visada leisti pranešimus** iš šių IP adresų arba adresų diapazono ir sužinokite, **ar pasirinkta Įjungti saugų** sąrašą.

   > [!NOTE]
   > "Microsoft" prenumeruoja trečiųjų šalių patikimų siuntėjų šaltinius. Jei įgalintas saugus sąrašas, šie patikimi siuntėjai klaidingai nepažymimi kaip pašto šiukšlės. Rekomenduojame pasirinkti šią parinktį, nes ji sumažins gautų klaidingai teigiamų laiškų (gerų laiškų, kurie klasifikuojami kaip pašto šiukšlės) skaičių.

Daugiau informacijos žr. [Ryšio filtravimo konfigūravimas](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
