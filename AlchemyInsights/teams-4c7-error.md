---
title: "\"Teams\" 4c7 klaida"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796248"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 klaida "Microsoft teams"

Ši klaida įvyksta, nes "Microsoft teams" reikalingas formų autentifikavimas. Kai diegiate Active Directory susiejimo tarnyba (AD FS), formų autentifikavimas neįgalintas intraneto pagal numatytuosius parametrus. Jei "Windows" integruotasis autentifikavimas nepavyksta, būsite paraginti prisijungti naudodami formų autentifikavimas.

Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimas naudojant AD FS Microsoft valdymo konsolės (MMC) pridėtiniame įrankyje kompiuteryje, kuriame yra vietos kopiją Active Directory. Jei norite tai padaryti, atlikite tokius veiksmus: 

1. Naršymo srityje suraskite **autentifikavimo strategijos**.
2. Dalyje **veiksmai** išsamios informacijos srityje pasirinkite **Redaguoti visuotinį pirminį autentifikavimą**.
3. Skirtuke **intranetas** pasirinkite **formų autentifikavimas**.
4. Pasirinkite **gerai** (arba **taikyti**).