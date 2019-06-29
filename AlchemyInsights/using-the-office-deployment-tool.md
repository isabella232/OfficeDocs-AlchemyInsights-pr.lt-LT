---
title: Naudodami Office diegimo įrankis
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365533"
---
# <a name="using-the-office-deployment-tool-odt"></a>Naudodami Office diegimo įrankis (ODT)

Diegiate "Office 365" "Office" versijos naudodami Office diegimo įrankis (ODT). Office diegimo įrankis (setup.exe) yra paleisti iš komandinės eilutės ir naudoja XML konfigūracijos failo nustatyti, kokius parametrus taikyti, kai diegiant Office.
  
1. Atsisiųsti naujausią versiją Office diegimo įrankis iš [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Naudokite [Office tinkinimo įrankį (UŠT)](https://config.office.com) pasirinkti diegimo nuostatas ir sukurkite XML konfigūracijos failo. Eksportuoti konfigūracijos failą ir įdėkite jį vietoje ant tame pačiame aplanke, kur gyvena ant "setup.exe".

    **Pastaba:** Office diegimo problemos dažniausiai atsiranda dėl į klaidingai arba malformatted konfigūracijos failus. Siekiant išvengti tokių problemų, mes rekomenduojame, kad naudojate Office tinkinimo įrankį Norėdami sukurti konfigūracijos failą. Taip pat galite importuoti esamą konfigūracijos failus į Office tinkinimo įrankį.

3. Didesnių teisių komandų eilutėje, persijunkite į tą vietą, kurioje gyvena setup.exe ir paleisti Office diegimo įrankis atsisiųsti režimu ir nurodykite konfigūracijos failą išsaugoti. Šiame pavyzdyje konfigūracijos failas pavadintas Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Paleisti Office diegimo įrankis, konfigūruoti režimu ir nustatyti konfigūracijos failą.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Pastaba:** Šį veiksmą turite paleisti iš kliento kompiuteryje, kuriame norite įdiegti "Office" ir tame kompiuteryje turite turėti vietos administratoriaus teises.

Norėdami sužinoti daugiau apie jūsų "Office 365 ProPlus" visuotinio diegimo scenarijai naudojant Office diegimo įrankis, ieškokite [apžvalga Office diegimo įrankis](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Daugiau informacijos apie tai, kaip naudoti Office tinkinimo įrankį, žr [apžvalga Office tinkinimo įrankį](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
