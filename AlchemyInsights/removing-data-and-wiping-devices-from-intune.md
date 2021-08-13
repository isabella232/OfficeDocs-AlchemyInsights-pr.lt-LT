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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922247"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Duomenų šalinimas ir įrenginių duomenų ištrynimas iš „Intune“

Norint pašalinti įmonės duomenis, valdomus „Intune“, arba atkurti gamyklinius parametrus ir grąžinti įrenginio numatytuosius parametrus, galima naudoti nuotolinius veiksmus Nustoti naudoti įrenginį ir Įrenginio duomenų ištrynimas.

1. Prisijunkite prie ataskaitų srities „Microsoft 365“ įrenginių valdymas ir eikite į sritį **Įrenginiai,** > **Visi įrenginiai**.
2. Pasirinkite įrenginį, kurio duomenis norite ištrinti.
3. Pasirinkite norimo atlikti nuotolinio ištrynimo tipą. Funkcija Nustoti naudoti panaikina tik organizacijos informaciją, o tuo tarpu visiškas duomenų ištrynimas atkuria įrenginio gamyklinius parametrus.
4. Patvirtinkite pasirinkdami **Taip**. Iki tol, kol ištrynimo veiksmas bus baigtas, įrenginio veiksmo būsena bus rodoma kaip *Laukiama, kol bus nustota naudoti*.
    Atlikus veiksmą, mobiliojo įrenginio nebematysite valdomųjų įrenginių sąraše.

> [!NOTE]
> Įmonės duomenų negalima pašalinti iš įrenginių, PRIJUNGTŲ prie „Microsoft Azure AD“. 

Visą išsamią informaciją apie veiksmų Nustoti naudoti ir Duomenų ištrynimas poveikį, įskaitant tai, kas paliekama ir kas panaikinama, žr. šiuose dokumentuose:

- [Įrenginių pašalinimas naudojant duomenų ištrynimo ir nustojimo naudoti funkcijas arba rankiniu būdu išregistruojant įrenginį](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kaip iš „Intune“ valdomų programų ištrinti tik įmonės duomenis](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Visų duomenų ištrynimas iš „MacOS“ įrenginio](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).