---
title: "\"Intune\" sąlyginės prieigos stebėjimas"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427923"
---
# <a name="monitor-intune-conditional-access"></a>"Intune" sąlyginės prieigos stebėjimas

Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų. Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:

1. Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale. Jei ne, vartotojas turi užregistruoti įrenginį.
1. "Azure" portale eikite į " **Intune**"  >  **įrenginio atitiktį**. 
1. Norėdami peržiūrėti įrenginio atitikties ataskaitą, kad įsitikintumėte, jog vartotojo įrenginys pažymėtas kaip suderinamas, dalyje **monitorius** spustelėkite **įrenginio atitiktis**.
1. "Azure" portale eikite į " **Intune**"  >  **įrenginio atitiktį**. Dalyje **tvarkyti** spustelėkite **strategijos**. Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui. Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos.
1. Vartotojo sąlyginės prieigos priskyrimo redagavimas.
1. "Azure" portale eikite į **Intune**  >  **sąlyginės prieigos**  >  **strategijas**, iš sąrašo pasirinkite strategiją ir spustelėkite **vartotojai ir grupės**.
1. Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į **sąrašą įtraukti**. Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į **sąrašą neįtraukti**.

**Naudingi saitai:**

- [Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Trikčių diagnostika CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Trikčių šalinimo strategija](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- ["Intune" įrenginio atitikties stebėjimas](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Šie veiksmai yra naudingi šalinant "Azure Active Directory" funkcijos sąlyginę prieigą. Taip pat galima sulaikyti įrenginį, kuris blokuoja prieigą prie "Exchange" strategijos. Daugiau informacijos apie "Exchange" įrenginių valdymą rasite [**čia**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
