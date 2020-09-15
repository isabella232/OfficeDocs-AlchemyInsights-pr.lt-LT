---
title: Sąlyginės prieigos stebėjimas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702911"
---
# <a name="monitoring-conditional-access-for-exchange"></a>"Exchange" sąlyginės prieigos stebėjimas

Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų. Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:
  
- Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale. Jei ne, vartotojas turi registruotis įrenginyje.
    
- "Azure" portale eikite į " **Intune" \> įrenginio atitiktį**. Dalyje **monitorius** spustelėkite **įrenginio atitiktis**. Peržiūrėkite savo įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas. 
    
- "Azure" portale eikite į " **Intune" \> įrenginio atitiktį**. Dalyje **tvarkyti**spustelėkite **strategijos**. Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui. Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos. 
    
- Vartotojo sąlyginės prieigos priskyrimo redagavimas.
    
1. "Azure" portale eikite į " **Intune" \> sąlyginės prieigos \> strategijas**
    
2. Sąraše pasirinkite strategiją
    
3. Spustelėkite **vartotojai ir grupės**
    
4. Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į sąrašą **įtraukti** . Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į sąrašą **neįtraukti** . 
    
Skaitykite daugiau: [kaip stebėti sąlyginės prieigos įrenginius](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

