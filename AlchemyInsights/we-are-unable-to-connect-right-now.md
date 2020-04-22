---
title: Aktyvinimo problema - Mes negalime prisijungti dabar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716180"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>"Office" programų "Šiuo metu nepavyksta prisijungti" nustatymas

Jei gaunate šį pranešimą, pabandykite atlikti šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Office" programų. Peržiūrėkite ["Microsoft" URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite į **Pradėti** > **vykdyti**, tada įveskite **services.msc**. Įsitikinkite, kad visos šios tarnybos veikia:
    - Tinklo prijungtų įrenginių automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vietos žinomumas
    - Windows įvykių žurnalas

Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti. Jei kyla problemų paleidžiant tarnybą, atidarę komandinę eilutę su didesnių teisių komanda vykdykite šią komandą:

**SFC /scannow SFC /scannow SFC / scannow SFC**

Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.

Išsamesnės informacijos [ieškokite "Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai aktyvinate "Office" iš "Microsoft 365".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)