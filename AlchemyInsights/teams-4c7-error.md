---
title: "\"Teams 4c7\" klaida"
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786677"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 klaida "Microsoft Teams"

Ši klaida įvyksta todėl, kad "Microsoft Teams" reikalauja formų autentifikavimo. Kai diegiate "Active Directory" susiejimo tarnybas (AD FS), formų autentifikavimas intranete pagal numatytuosius parametrus neįgalintas. Jei "Windows" integruotasis autentifikavimas nepavyksta, būsite paraginti prisijungti naudodami formų autentifikavimą.

Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimą naudodami AD FS "Microsoft" valdymo konsolės (MMC) pridėtinį įrankį kompiuteryje, kuriame yra vietinė "Active Directory" kopija. Jei norite tai padaryti, atlikite tokius veiksmus: 

1. Naršymo srityje raskite **Autentifikavimo strategijos**.
2. Išsamios **informacijos** srityje dalyje Veiksmai pasirinkite Redaguoti **visuotinį pirminį autentifikavimą**.
3. Skirtuke **Intranetas** pasirinkite Formų **autentifikavimas**.
4. Pasirinkite **Gerai** (arba **Taikyti**).