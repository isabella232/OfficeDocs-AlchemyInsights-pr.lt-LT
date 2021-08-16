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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988124"
---
# <a name="fix-connection-policy"></a>Ryšio strategijos taisymas

El. laiškas buvo pažymėtas saugus ir pristatytas į vartotojo aplanką Gauta, nes siuntimo IP adresas buvo pažymėtas kaip saugus ryšio filtro politikoje. Norėdami peržiūrėti strategiją, atlikite šiuos veiksmus:

1. Eikite į [Office 365 saugos & centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143), tada eikite į **Grėsmių valdymo strategija** Apsauga  >  **nuo** pašto  >  [šiukšlių](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Skirtuke **Pasirinktinis** pasirinkite **ryšio filtro strategiją**, tada pasirinkite Redaguoti **strategiją**.
3. Peržiūrėkite **SĄRAŠĄ LEISTI IP.** **Sužinokite, Seifas įgalintas** sąrašas.

    > [!NOTE]
    > "Microsoft" prenumeruoja trečiųjų šalių patikimų siuntėjų šaltinius. Jei **Seifas,** šie patikimi siuntėjai klaidingai nepažymimi kaip pašto šiukšlės. Rekomenduojame pasirinkti šią parinktį, nes ji sumažins gautų klaidingų teigiamų laiškų (gerų laiškų, kurie klasifikuojami kaip pašto šiukšlės) skaičių.
