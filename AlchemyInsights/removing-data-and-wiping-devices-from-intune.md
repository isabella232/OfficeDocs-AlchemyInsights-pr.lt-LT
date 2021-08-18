---
title: Duomenų šalinimas ir įrenginių duomenų ištrynimas iš „Intune“
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331049"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Duomenų šalinimas ir įrenginių duomenų ištrynimas iš „Intune“

Norint pašalinti įmonės duomenis, valdomus „Intune“, arba atkurti gamyklinius parametrus ir grąžinti įrenginio numatytuosius parametrus, galima naudoti nuotolinius veiksmus Nustoti naudoti įrenginį ir Įrenginio duomenų ištrynimas.

1. Prisijunkite prie ataskaitų srities „Microsoft 365“ įrenginių valdymas ir eikite į sritį **Įrenginiai,** > **Visi įrenginiai**.
2. Pasirinkite įrenginį, kurio duomenis norite ištrinti.
3. Pasirinkite norimo atlikti nuotolinio ištrynimo tipą. Funkcija Nustoti naudoti panaikina tik organizacijos informaciją, o tuo tarpu visiškas duomenų ištrynimas atkuria įrenginio gamyklinius parametrus.
4. Patvirtinkite pasirinkdami **Taip**. Iki tol, kol ištrynimo veiksmas bus baigtas, įrenginio veiksmo būsena bus rodoma kaip *Laukiama, kol bus nustota naudoti*.
    Atlikus veiksmą, mobiliojo įrenginio nebematysite valdomųjų įrenginių sąraše.

**Pastaba:** įmonės duomenų negalima pašalinti iš įrenginių, PRIJUNGTŲ prie "Azure AD". 

Visą išsamią informaciją apie veiksmų Nustoti naudoti ir Duomenų ištrynimas poveikį, įskaitant tai, kas paliekama ir kas panaikinama, žr. šiuose dokumentuose:

- [Įrenginių pašalinimas naudojant duomenų ištrynimo ir nustojimo naudoti funkcijas arba rankiniu būdu išregistruojant įrenginį](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kaip iš „Intune“ valdomų programų ištrinti tik įmonės duomenis](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Visų duomenų ištrynimas iš „MacOS“ įrenginio](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).