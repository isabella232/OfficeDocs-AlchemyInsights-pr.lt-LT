---
title: "\"Office\" diegimo įrankio naudojimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083778"
---
# <a name="using-the-office-deployment-tool-odt"></a>"Office" diegimo įrankio (ODT) naudojimas

Galite naudoti Office diegimo įrankį (ODT), kad įdiegtų Office 365 "Office" versijas. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.
  
1. Atsisiųskite naujausią "Office diegimo įrankio versiją iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Naudokite [Office tinkinimo įrankį (OCT),](https://config.office.com) kad pasirinktumėte diegimo nuostatas ir sukurtumėte konfigūracijos XML failą. Eksportuokite konfigūracijos failą ir padėkite jį vietoje tame pačiame aplanke, kuriame setup.exe vieta.

    **Pastaba:** Office diegimo problemos dažniausiai kyla dėl netinkamai sukonfigūruotų arba netinkamai suformatuotos konfigūracijos failų. Norėdami išvengti tokių problemų, rekomenduojame naudoti Office tinkinimo įrankį, kad sukurtumėte konfigūracijos failą. Taip pat galite importuoti esamus konfigūracijos failus į Office tinkinimo įrankį.

3. Didesnių teisių komandinėje eilutėje pereikite į vietą, kurioje yra "setup.exe" ir paleiskite "Office" diegimo įrankį atsisiuntimo režimu ir nurodykite ką tik įrašytą konfigūracijos failą. Šiame pavyzdyje konfigūracijos failas pavadintas Configuration.xml:

```setup.exe /download Configuration.xml```

4.Paleiskite Office diegimo įrankį konfigūravimo režimu ir nurodykite konfigūracijos failą.

```setup.exe /configure Configuration.xml```

**Pastaba:** Turite atlikti šį veiksmą iš kliento kompiuterio, kuriame norite įdiegti "Office ir turite turėti vietinio administratoriaus teises šiame kompiuteryje.

Norėdami sužinoti daugiau apie "Office" diegimo įrankio "Microsoft 365" programos įmonėms diegimo scenarijus, [žr. "Office" diegimo įrankio apžvalga.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Daugiau informacijos apie tai, kaip naudoti Office tinkinimo įrankį, [žr. "Office tinkinimo įrankio apžvalga.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
