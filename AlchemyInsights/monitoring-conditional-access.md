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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708682"
---
# <a name="monitoring-conditional-access-for-exchange"></a>"Exchange" sąlyginės prieigos stebėjimas

Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų. Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:

- Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale. Jei ne, vartotojas turi registruotis įrenginyje.
- "Azure" portale eikite į Intune > įrenginio atitiktis. Dalyje monitorius spustelėkite įrenginio atitiktis. Peržiūrėkite savo įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas.
- "Azure" portale eikite į Intune > įrenginio atitiktis. Dalyje tvarkyti spustelėkite strategijos. Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui. Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos.
- Vartotojo sąlyginės prieigos priskyrimo redagavimas.

1. "Azure" portale eikite į " **Intune**"  >  **sąlyginės prieigos**  >  **strategijas**.
2. Sąraše pasirinkite strategiją.
3. Spustelėkite vartotojai ir grupės.
4. Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į sąrašą įtraukti. Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į sąrašą neįtraukti.

Naudingi saitai:

[Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)

[Trikčių diagnostika CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Trikčių šalinimo strategija](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

["Intune" įrenginio atitikties stebėjimas](https://docs.microsoft.com/intune/compliance-policy-monitor)

Pastaba: šie veiksmai naudingi tik šalinant "Azure Active Directory" funkcijos sąlyginę prieigą. Taip pat galima sulaikyti įrenginį, kuris blokuoja prieigą prie "Exchange" strategijos. Daugiau informacijos apie "Exchange" įrenginių valdymą galima rasti [čia] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
