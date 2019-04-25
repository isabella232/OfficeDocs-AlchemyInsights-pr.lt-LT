---
title: Stebėsenos sąlyginės prieigos
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418477"
---
# <a name="monitoring-conditional-access"></a>Stebėsenos sąlyginės prieigos

Vartotojams skirta su sąlygine prieiga gausite pranešimas el. paštu, jei jie neatitinka jūsų organizacijos suteikiant prieigą keliami reikalavimai. Norėdami išspręsti, rekomenduojame vieną ar kelis iš šių sprendimų:
  
- Jei prietaisas yra preziumuojamas, gautų, patarti vartotojui eiti į programėlę įmonės portalą ir patikrinkite, ar rodomas įmonės portale. Jei ne, vartotojas turėtų registruotis įrenginį.
    
- Azure portale rasite apsilankę **Intune \> prietaiso atitikties**. Po **monitoriumi** spustelėkite **įrenginio atitiktį**. Rodyti jūsų prietaiso atitikties ataskaitą, kad patikrinti, kad vartotojo įrenginys pažymimas kaip suderinamas. 
    
- Azure portale rasite apsilankę **Intune \> prietaiso atitikties**. Dalyje **tvarkyti**spustelėkite **strategijos**. Atitikties strategijos sąraše, patikrinkite, kad profilis yra priskirtas jūsų vartotojo įrenginio. Jei nėra Vartotojo profilis yra priskirtas, tada Intune nebus galima patvirtinti įrenginio atitikties būklę. 
    
- Redaguoti vartotojo sąlyginės prieigos priskyrimo.
    
1. Azure portale rasite apsilankę **Intune \> sąlyginės prieigos \> politika**
    
2. Iš sąrašo pasirinkite politiką
    
3. Spustelėkite **vartotojai ir grupės**
    
4. Nukreipti tam tikrą politiką kažkas, įtraukti juos į sąrašus **įtraukti** . Siekiant užtikrinti, kad asmuo yra praleista politiką, įtraukti juos į sąrašą **neįtraukti** . 
    
Skaityti daugiau: [kaip stebėti sąlyginės prieigos priemonės](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

