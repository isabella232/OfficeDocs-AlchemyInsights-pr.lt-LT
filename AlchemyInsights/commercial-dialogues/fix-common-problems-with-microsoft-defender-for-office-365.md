---
title: Dažniausiai pasitaikančių "Microsoft" sargybos problemų sprendimas Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330068"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Dažniausiai pasitaikančių "Microsoft" sargybos problemų sprendimas Office 365

Toliau pateikiami keli dažniausiai pasitaikančių "Microsoft" sargybos problemų Office 365:

- **Pranešimo delsa**:

  El. laiškų pristatymo delsą gali sukelti Seifas priedų nuskaitymas. Daugiau informacijos žr. [Seifas priedų strategijos parametrai](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Pranešti apie klaidingus teigiamus arba neigiamus rezultatus:**

  Daugiau informacijos žr. [Pranešimas apie pranešimus ir failus "Microsoft".](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Įjungti Seifas saito apsaugą:**

  1. ""Microsoft 365" sargyba" portale eikite į El. & bendradarbiavimo <https://security.microsoft.com/> strategijos &  \> **Grėsmių** strategijos Seifas \>  \> **saitai** **dalyje** Strategijos.

     Norėdami pereiti tiesiai į **Seifas saitų puslapį,** naudokite <https://security.microsoft.com/safelinksv2> .

  2. Puslapyje **Seifas** saitai pasirinkite strategiją spustelėdami strategijos pavadinimą.
  3. Rodomame išsamios informacijos iškeliame meniu atlikite vieną iš šių veiksmų:
     - Norėdami įtraukti naują strategiją, pasirinkite **+ Kurti**. Bus paleidžiamas vediklis, kuris padės nustatyti strategijos parametrus.
     - Norėdami redaguoti esamą strategiją, pasirinkite strategiją spustelėdami strategijos pavadinimą. Rodomame išsamios informacijos iškeliame lange **pasirinkite Redaguoti** **sekcijoje Apsaugos** parametrai.
  4. Puslapyje **Apsaugos parametrai** sukonfigūruokite šiuos parametrus:
     - Įjunkite **Pasirinkite veiksmą, jei laiškuose yra nežinomų potencialiai kenkėjiškų URL**.
     - Pasirinkite **Taikyti saugius saitus organizacijos siunčiamims laiškams.**

  Daugiau informacijos žr. [Saitų strategijų Seifas "Microsoft" sargyba, Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
