---
title: Saugojimo strategijos "Exchange" administravimo centre neveikia
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952236"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Saugojimo strategijos "Exchange" administravimo centre

Jei norite, kad atliktų toliau nurodytų parametrų automatinį patikrinimą, šio puslapio viršuje pasirinkite mygtuką atgal <- ir įveskite vartotojo, kuris susiduria su saugojimo strategijų problemomis, el. pašto adresą.

Jei kyla problemų dėl saugojimo strategijų "Exchange" administravimo centre, kurie nėra taikomi pašto dėžutėms arba elementams, kurie nėra perkeliami į archyvo pašto dėžutę, patikrinkite šiuos dalykus:

**Pagrindinės priežastys:**

- **Valdomų aplankų** asistentas ne apdorojo vartotojo pašto dėžutės. Valdomų aplankų pagalbinė priemonė bando apdoroti kiekvieną pašto dėžutę debesies pagrindu pagrįstoje organizacijoje kartą per septynias dienas.

  **Sprendimas:** Paleiskite valdomų aplankų pagalbinę priemonę.

- **Saugojimolaikymas** **įgalintas** pašto dėžutėje. Jei pašto dėžutė buvo įdedama į saugojimo saugyklą, tuo metu pašto dėžutės saugojimo strategija nebus apdorojama.

  **Sprendimas:** Patikrinkite saugojimo sulaikymo parametro būseną ir atnaujinkite, jei reikia. Daugiau informacijos žr. [Pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Pastaba:** Jei pašto dėžutė mažesnė nei 10 MB, valdomų aplankų asistentas pašto dėžutės automatiškai ne apdoros.
 
Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre žr.:

- [Saugojimo žymės ir saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Saugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) arba [Saugojimo žymių įtraukimas arba pašalinimas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kaip nustatyti pašto dėžutėje laikomos sulaikytos vietos tipą](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
