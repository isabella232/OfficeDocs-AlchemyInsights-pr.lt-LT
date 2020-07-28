---
title: Duomenų ir valymo įrenginių šalinimas iš "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439645"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Duomenų ir valymo įrenginių šalinimas iš "Intune"

Įrenginio išėjimo į pensiją ir įrenginio ištrynimo nuotoliniai veiksmai gali būti naudojami pašalinti "Intune" valdomus įmonės duomenis arba atlikti gamyklinius nustatymus ir grąžinti įrenginio numatytuosius parametrus.

1. Prisijunkite prie "Microsoft 365" įrenginių valdymo ir eikite į **Įrenginiai**  >  **visi įrenginiai**.
2. Pasirinkite įrenginį, kurį norite ištrinti.
3. Pasirinkite nuotolinio ištrynimo tipą, kurį norite atlikti. Išeinant į pensiją ištrina tik organizacinę informaciją, o visi servetėlės atkurti įrenginio gamyklinius nustatymus.
4. Pasirinkite **Taip,** kad patvirtintumėte. Kol valymas bus baigtas, įrenginio veiksmo būsena rodoma kaip Laukiama.</br>
    Kai veiksmas bus baigtas, valdomo įrenginio sąraše mobiliojo įrenginio nebematysite.

**Pastaba** Įmonės duomenų negalima pašalinti iš įrenginių, prijungtų prie "Azure AD".

Išsamią informaciją apie veiksmų "Išeiti į pensiją ir ištrynimas" poveikį, įskaitant tai, kas išlaikoma ir kas ištrinama, rasite [Įrenginių šalinimas naudojant ištrynimą, išeikite į pensiją arba rankiniu būdu išpakuodami įrenginį](https://docs.microsoft.com/intune/devices-wipe).

Norėdami ištrinti visus duomenis iš "macOS" įrenginio, [žr.](https://docs.microsoft.com/intune/device-erase)