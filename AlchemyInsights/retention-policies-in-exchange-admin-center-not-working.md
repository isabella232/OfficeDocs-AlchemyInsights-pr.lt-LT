---
title: Saugojimo strategijos Exchange administravimo centre neveikia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074940"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saugojimo strategijos Exchange administravimo centre

Jei norite, kad atliktų toliau nurodytų parametrų automatinį patikrinimą, šio puslapio viršuje pasirinkite mygtuką atgal <- ir įveskite vartotojo, kuris susiduria su saugojimo strategijų problemomis, el. pašto adresą.

Jei kyla problemų dėl saugojimo strategijų "Exchange administravimo centre, netaikoma pašto dėžutėms ar elementams, kurie nėra perkeliami į archyvo pašto dėžutę, patikrinkite šiuos dalykus:

**Pagrindinės priežastys:**

- **Valdomų aplankų** asistentas ne apdorojo vartotojo pašto dėžutės. Valdomų aplankų pagalbinė priemonė bando apdoroti kiekvieną pašto dėžutę debesies pagrindu pagrįstoje organizacijoje kartą per septynias dienas.

  **Sprendimas:** Paleiskite valdomų aplankų pagalbinę priemonę.

- **Saugojimolaikymas** **įgalintas** pašto dėžutėje. Jei pašto dėžutė buvo įdedama į saugojimo saugyklą, tuo metu pašto dėžutės saugojimo strategija nebus apdorojama.

  **Sprendimas:** Patikrinkite saugojimo sulaikymo parametro būseną ir atnaujinkite, jei reikia. Daugiau informacijos žr. [Pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Pastaba:** Jei pašto dėžutė mažesnė nei 10 MB, valdomų aplankų asistentas pašto dėžutės automatiškai ne apdoros.
 
Daugiau informacijos apie saugojimo strategijas Exchange administravimo centre, žr.:

- [Saugojimo žymės ir saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Saugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) arba [Saugojimo žymių įtraukimas arba pašalinimas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kaip nustatyti pašto dėžutėje laikomos sulaikytos vietos tipą](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
