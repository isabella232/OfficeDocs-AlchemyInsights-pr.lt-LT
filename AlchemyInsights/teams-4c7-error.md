---
title: Teams 4c7 klaida
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049316"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 klaida Microsoft Teams

Ši klaida įvyksta dėl Microsoft Teams formų autentifikavimo. Kai diegiate "Active Directory" susiejimo tarnybas (AD FS), formų autentifikavimas intranete pagal numatytuosius parametrus neįgalintas. Jei Windows autentifikavimas nepavyksta, būsite paraginti prisijungti naudodami formų autentifikavimą.

Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimą naudodami AD FS "Microsoft" valdymo konsolės (MMC) pridėtinį įrankį kompiuteryje, kuriame yra vietinė "Active Directory" kopija. Jei norite tai padaryti, atlikite tokius veiksmus: 

1. Naršymo srityje raskite **Autentifikavimo strategijos**.
2. Išsamios **informacijos** srityje dalyje Veiksmai pasirinkite Redaguoti **visuotinį pirminį autentifikavimą**.
3. Skirtuke **Intranetas** pasirinkite Formų **autentifikavimas**.
4. Pasirinkite **Gerai** (arba **Taikyti**).