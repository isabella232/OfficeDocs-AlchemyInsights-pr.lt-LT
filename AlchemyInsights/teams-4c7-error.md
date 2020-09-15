---
title: "\"Teams\" 4c7 klaida"
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700211"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 klaida programoje "Microsoft teams"

Ši klaida įvyksta dėl to, kad "Microsoft teams" reikia formų autentifikavimo. Kai diegiate "Active Directory" susiejimo tarnybą (AD FS), intraneto formų autentifikavimas neįgalintas pagal numatytuosius. Jei nepavyksta "Windows" integruoto autentifikavimo, būsite paraginti prisijungti naudodami formų autentifikavimą.

Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimą naudodami AD FS "Microsoft" valdymo konsolės (MMC) pridėtinį įrankį kompiuteryje, kuriame yra vietinė "Active Directory" kopija. Jei norite tai padaryti, atlikite tokius veiksmus: 

1. Naršymo srityje raskite **autentifikavimo strategijas**.
2. Dalyje **veiksmai** išsamios informacijos srityje pasirinkite **Redaguoti visuotinį pirminį autentifikavimą**.
3. Skirtuke **intranetas** pasirinkite **formų autentifikavimas**.
4. Pasirinkite **gerai** (arba **taikyti**).