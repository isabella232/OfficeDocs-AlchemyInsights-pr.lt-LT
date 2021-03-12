---
title: Nuomotojo strategijos taisymas (veiksmo nepaisymas)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748995"
---
# <a name="fix-tenant-policy-action-override"></a>Nuomotojo strategijos taisymas (veiksmo nepaisymas)

"Anti-spam" strategija jūsų nuomotojuje paveikė šį pranešimą. Norėdami peržiūrėti strategiją, atlikite šiuos veiksmus:

1. Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143), tada eikite į **grėsmių valdymo**  >  **strategija**  >  [apsauga nuo pašto šiukšlių](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Patikrinkite, ar **strategijos šaltinis** nurodo:  **Add-XHeader/Modifysubject/peradresavimo/naikinimo/nėra veiksmų/BCC pranešimas**

    Jei taip, skirtuke **Pasirinktinai** patikrinkite strategijos, kuri paveikė laišką, parametrus. Gali būti, kad **standartiniai parametrai** , taikomi visiems "Exchange Online Protection" klientams, paveikė laišką.

Daugiau informacijos apie pašto šiukšlių filtravimo strategijų konfigūravimą rasite [pašto šiukšlių filtravimo strategijų](https://go.microsoft.com/fwlink/?linkid=2101431)konfigūravimas.
