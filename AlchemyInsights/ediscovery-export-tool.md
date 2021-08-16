---
title: El. duomenų aptikimo eksportavimo įrankis
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101310"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Negalite įdiegti arba paleisti el. duomenų aptikimo eksportavimo įrankio?

Jei negalite įdiegti arba paleisti el. duomenų aptikimo eksportavimo įrankio, kad atsisiųstumėte ieškos rezultatus, patikrinkite šiuos dalykus:
  
- Jūsų naudojamas kompiuteris atitinka šiuos išankstinius reikalavimus:

  - 32 arba 64 bitų "Windows 7" ir naujesnės versijos

  - „Microsoft .NET Framework 4.7“

  - Palaikoma naršyklė:

  - „Microsoft Edge“

    Arba

  - Internet Explorer 10 ir naujesnės versijos

    Kitos naršyklės, pvz., "Google Chrome" ir "Mozilla Firefox", nepalaikomos.

- Jūsų organizacija gali prisijungti prie pabaigos taško "Azure", **\* kuris yra .blob.core.windows.net** (pakaitos ženklas nurodo unikalų eksportavimo užduoties identifikatorių).

- Jums priskirtas eksportavimo vaidmuo Microsoft 365 atitikties &amp; centre. Pagal numatytuosius nustatymus šis vaidmuo priskiriamas tik el. duomenų aptikimo tvarkytuvo vaidmenų grupei. Žr. [El. duomenų aptikimo teisių priskyrimas](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Daugiau informacijos žr. [Turinio ieškos rezultatų eksportavimas](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Jei eksportuojate daugiau nei 100 K pašto dėžutes, norėdami atsisiųsti eksportavimo rezultatus, turėsite naudoti šią "Powershell": Rezultatų eksportavimas iš daugiau nei [100K pašto dėžučių.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)