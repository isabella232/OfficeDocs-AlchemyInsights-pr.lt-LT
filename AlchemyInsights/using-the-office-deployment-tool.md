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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794919"
---
# <a name="using-the-office-deployment-tool-odt"></a>"Office" diegimo įrankio naudojimas (ODT)

Naudokite "Office" diegimo įrankį (ODT), kad įdiegtumėte "Office 365" versijas "Office". "Office" diegimo įrankis (setup.exe) paleidžiamas iš komandų eilutės ir naudoja konfigūracijos XML failą, kad nustatytų, kokie parametrai turi būti taikomi diegiant "Office".
  
1. Atsisiųskite naujausią "Office" diegimo įrankio versiją iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Naudokite " [Office" tinkinimo įrankį (OCT)](https://config.office.com) , kad pasirinktumėte diegimo nuostatas ir SUKURTUMĖTE konfigūracijos XML failą. Eksportuokite konfigūracijos failą ir padėkite jį vietiniame tame pačiame aplanke, kuriame yra setup.exe.

    **Pastaba:** "Office" diegimo problemos paprastai kyla dėl netinkamai sukonfigūruotų arba netinkamai suformatuotų konfigūracijos failų. Norėdami išvengti tokių problemų, rekomenduojame naudoti "Office" tinkinimo įrankį kuriant konfigūracijos failą. Esamus konfigūracijos failus taip pat galite importuoti į "Office" tinkinimo įrankį.

3. Didesnių teisių komandų eilutėje įjunkite vietą, kurioje setup.exe gyvena, ir paleiskite "Office" diegimo įrankį atsisiuntimo režimu ir nustatykite ką tik įrašytą konfigūracijos failą. Šiame pavyzdyje konfigūracijos failas pavadintas Configuration.xml:

```setup.exe /download Configuration.xml```

4. Paleiskite "Office" diegimo įrankį konfigūravimo režimu ir nustatykite konfigūracijos failą.

```setup.exe /configure Configuration.xml```

**Pastaba:** Šį veiksmą turite atlikti iš kliento kompiuterio, kuriame norite įdiegti "Office", ir tame kompiuteryje turite turėti vietinio administratoriaus teises.

Norėdami sužinoti daugiau apie "Office" diegimo įrankio naudojimą "Microsoft" 365 programoms, skirtas įmonės diegimo scenarijams, skaitykite " [Office" diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Daugiau informacijos, kaip naudoti "Office" tinkinimo įrankį, rasite " [Office" tinkinimo įrankio apžvalga](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
