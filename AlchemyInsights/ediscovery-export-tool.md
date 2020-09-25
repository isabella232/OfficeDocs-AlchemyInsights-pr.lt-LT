---
title: "\"Udiscovery\" eksportavimo įrankis"
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277922"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Nepavyksta įdiegti arba paleisti "Udiscovery" eksportavimo įrankio?

Jei negalite įdiegti arba paleisti "Udiscovery" eksportavimo įrankio, kad atsisiųstumėte ieškos rezultatus, patikrinkite šiuos dalykus:
  
- Jūsų naudojamas kompiuteris atitinka šias išankstines sąlygas:

  - "32" arba "64" bitų versijos "Windows 7" ir naujesnėse versijose

  - „Microsoft .NET Framework 4.7“

  - Palaikoma naršyklė:

  - "Microsoft Edge"

    Arba

  - "Internet Explorer 10" ir vėlesnės versijos

    Kitos naršyklės, pvz., "Google Chrome" ir "Mozilla Firefox", yra nepalaikomos.

- Jūsų organizacija gali prisijungti prie galinio punkto "Azure", kuris yra ** \* . BLOB.Core.Windows.net** (pakaitos simbolis nurodo unikalų jūsų eksportavimo užduoties identifikatorių).

- "Microsoft 365" saugos atitikties centre priskirtas eksportavimo vaidmuo &amp; . Pagal numatytuosius numatytuosius reikšmę šis vaidmuo priskiriamas tik "Udiscovery Manager" vaidmenų grupei. Žiūrėkite [priskirti elektroninės aptikimo teises](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Daugiau informacijos ieškokite [turinio ieškos rezultatų eksportavimas](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Jei eksportuojate daugiau nei 100 k pašto dėžučių, turite naudoti šį "PowerShell", kad atsisiųstumėte eksportavimo rezultatus:  [rezultatų eksportavimas iš daugiau nei 100 k pašto dėžučių](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).