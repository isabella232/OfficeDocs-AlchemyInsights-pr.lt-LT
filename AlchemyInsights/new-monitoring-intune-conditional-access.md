---
title: Monitor Intune Conditional Access
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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025510"
---
# <a name="monitor-intune-conditional-access"></a>Monitor Intune Conditional Access

Vartotojai, kuriems skirta sąlyginė prieiga, gaus pranešimo el. laišką, jei jie neatitinka jūsų organizacijos prieigos reikalavimų. Norėdami išspręsti problemą, rekomenduojame vieną ar daugiau iš šių sprendimų:

1. Jei manoma, kad įrenginys yra įtrauktas į registrą, pateikite vartotojui Company Portal programėlę ir patikrinkite, ar jis rodomas Company Portal. Jei taip nėra, vartotojas turi užregistruoti įrenginį.
1. "Azure" portale eikite į **"Intune"**  >  **įrenginio atitiktis**. 
1. Norėdami peržiūrėti įrenginio atitikties ataskaitą ir patikrinti, ar vartotojo įrenginys pažymėtas kaip suderinamas, dalyje **Stebėti** spustelėkite **Įrenginio atitiktis**.
1. "Azure" portale eikite į **"Intune"**  >  **įrenginio atitiktis**. Dalyje **Valdyti spustelėkite** **Strategijos**. Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui. Jei profilis nepriskirtas, "Intune" negalės patvirtinti įrenginio atitikties būsenos.
1. Redaguokite vartotojo sąlyginės prieigos priskyrimą.
1. "Azure" portale eikite **į "Intune"** sąlyginės prieigos strategijos , sąraše pasirinkite strategiją  >    >  ir spustelėkite **Vartotojai ir grupės**.
1. Norėdami kam nors taikyti tam tikrą strategiją, įtraukite jas į **sąrašą Įtraukti**. Norėdami užtikrinti, kad asmuo būtų neįtrauktas į strategiją, įtraukite jį į **sąrašą Neįtraukti**.

**Naudingi saitai:**

- [Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)
- [CA trikčių diagnostika](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Trikčių diagnostikos strategija](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- ["Intune" įrenginio atitikties stebėjimas](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Šie veiksmai naudingi tik šalinant ""Azure Active Directory" sąlyginės prieigos triktis. Taip pat galima sulaikyti įrenginį, blokuojančią jo el. pašto prieigą, naudojant Exchange strategiją. Daugiau informacijos apie Exchange įrenginių valdymą rasite [**čia**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
