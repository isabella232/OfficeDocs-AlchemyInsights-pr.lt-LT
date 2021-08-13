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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975109"
---
# <a name="monitoring-conditional-access-for-exchange"></a>"Exchange

Vartotojai, kuriems skirta sąlyginė prieiga, gaus pranešimo el. laišką, jei jie neatitinka jūsų organizacijos prieigos reikalavimų. Norėdami išspręsti problemą, rekomenduojame vieną ar daugiau iš šių sprendimų:

- Jei manoma, kad įrenginys yra įtrauktas į registrą, pateikite vartotojui Company Portal programėlę ir patikrinkite, ar jis rodomas Company Portal. Jei taip nėra, vartotojas turėtų užregistruoti įrenginį.
- "Azure" portale eikite į "Intune" > įrenginio atitiktį. Dalyje Monitorius spustelėkite Įrenginio atitiktis. Peržiūrėkite įrenginio atitikties ataskaitą ir patikrinkite, ar vartotojo įrenginys pažymėtas kaip suderinamas.
- "Azure" portale eikite į "Intune" > įrenginio atitiktį. Dalyje Valdyti spustelėkite Strategijos. Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui. Jei profilis nepriskirtas, "Intune" negalės patvirtinti įrenginio atitikties būsenos.
- Redaguokite vartotojo sąlyginės prieigos priskyrimą.

1. "Azure" portale eikite į **"Intune"**  >  **sąlyginės prieigos**  >  **strategijos**.
2. Pasirinkite strategiją iš sąrašo.
3. Spustelėkite Vartotojai ir grupės.
4. Norėdami kam nors taikyti tam tikrą strategiją, įtraukite jas į sąrašą Įtraukti. Norėdami užtikrinti, kad asmuo būtų neįtrauktas į strategiją, įtraukite jį į sąrašą Neįtraukti.

Naudingi saitai:

[Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA trikčių diagnostika](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Trikčių diagnostikos strategija](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

["Intune" įrenginio atitikties stebėjimas](https://docs.microsoft.com/intune/compliance-policy-monitor)

Pastaba: šie veiksmai naudingi tik šalinant ""Azure Active Directory" sąlyginę prieigą. Taip pat galima sulaikyti įrenginį, blokuojančią jo el. pašto prieigą, naudojant Exchange strategiją. Daugiau informacijos apie Exchange įrenginių valdymą rasite [čia]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
