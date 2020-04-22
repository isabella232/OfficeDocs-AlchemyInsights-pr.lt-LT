---
title: Sąlyginės prieigos stebėjimas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713726"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Sąlyginės prieigos mainams stebėjimas

Vartotojai, kuriems taikoma sąlyginė prieiga, gaus pranešimo el. laišką, jei neatitinka jūsų organizacijos prieigos reikalavimų. Norėdami išspręsti, rekomenduojame vieną ar daugiau iš šių sprendimų:
  
- Jei manoma, kad įrenginys bus įtrauktas, patarkite vartotojui eiti į įmonės portalo programėlę ir patikrinti, ar jis rodomas įmonės portale. Jei ne, vartotojas turėtų užregistruoti įrenginį.
    
- Azure portale eikite į **Intune \> įrenginio atitiktis**. Dalyje **Monitorius** spustelėkite **Įrenginio atitiktis**. Peržiūrėkite įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas. 
    
- Azure portale eikite į **Intune \> įrenginio atitiktis**. Dalyje **Tvarkyti**spustelėkite **Strategijos**. Atitikties strategijų sąraše patikrinkite, ar jūsų vartotojo įrenginiui priskirtas profilis. Jei profilis nepriskirtas, "Intune" negalės patvirtinti įrenginio atitikties būsenos. 
    
- Redaguokite vartotojo sąlyginės prieigos priskyrimą.
    
1. Azure portale eikite į **Intune \> sąlyginės prieigos \> strategijos**
    
2. Pasirinkite strategiją iš sąrašo
    
3. Spustelėkite **Vartotojai ir grupės**
    
4. Norėdami taikyti pagal tam tikrą strategiją kam nors, įtraukite ją į sąrašą **Įtraukti.** Norėdami užtikrinti, kad asmuo nebūtų įtrauktas į strategiją, įtraukite jį į **sąrašą Neįtraukti.** 
    
Skaityti daugiau: [Kaip stebėti sąlyginės prieigos įrenginius](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

