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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366436"
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

[Trikčių šalinimo strategija](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

["Intune" įrenginio atitikties stebėjimas](https://docs.microsoft.com/intune/compliance-policy-monitor)

Pastaba: šie veiksmai naudingi tik šalinant "Azure Active Directory" funkcijos sąlyginę prieigą. Taip pat galima sulaikyti įrenginį, kuris blokuoja prieigą prie "Exchange" strategijos. Daugiau informacijos apie "Exchange" įrenginių valdymą rasite [čia](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
