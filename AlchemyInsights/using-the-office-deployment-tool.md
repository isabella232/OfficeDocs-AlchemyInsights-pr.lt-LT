---
title: "\"Office\" diegimo įrankio naudojimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726256"
---
# <a name="using-the-office-deployment-tool-odt"></a>"Office" diegimo įrankio (ODT) naudojimas

Galite naudoti Office visuotinio diegimo įrankis (ODT) diegti Office 365 versijos Office. "Office" visuotinio diegimo įrankis (setup.exe) vykdomas iš komandinės eilutės ir naudoja konfigūracijos XML failą, kad nustatytų, kokius parametrus taikyti diegiant "Office".
  
1. Atsisiųskite naujausią "Office" diegimo įrankio versiją iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Naudokite ["Office" tinkinimo įrankį (OCT),](https://config.office.com) kad pasirinktumėte diegimo nuostatas ir sukurtumėte konfigūracijos XML failą. Eksportuokite konfigūracijos failą ir padėkite jį vietiniame tame pačiame aplanke, kuriame yra setup.exe.

    **Pastaba:** "Office" diegimo problemos paprastai kyla dėl netinkamai sukonfigūruotų arba netinkamai suformatuotų konfigūracijos failų. Norėdami išvengti tokių problemų, rekomenduojame naudoti "Office" tinkinimo įrankį konfigūracijos failui sukurti. Taip pat galite importuoti esamus konfigūracijos failus į "Office" tinkinimo įrankį.

3. Didesnių teisių komandinėje eilutėje pereikite į vietą, kurioje yra setup.exe, ir paleiskite "Office" diegimo įrankį atsisiuntimo režimu ir nurodykite ką tik įrašytą konfigūracijos failą. Šiame pavyzdyje konfigūracijos failas pavadintas Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Paleiskite "Office" visuotinio diegimo įrankį konfigūravimo režimu ir nurodykite konfigūracijos failą.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Pastaba:** Šį veiksmą turite atlikti iš kliento kompiuterio, kuriame norite įdiegti "Office", ir tame kompiuteryje turite turėti vietinio administratoriaus teises.

Norėdami sužinoti daugiau apie "Office" diegimo įrankio naudojimą "Microsoft 365" programoms, skirtose įmonės diegimo scenarijams, [žr.](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool) Daugiau informacijos apie tai, kaip naudoti "Office" tinkinimo įrankį, ieškokite ["Office" tinkinimo įrankio apžvalga](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
