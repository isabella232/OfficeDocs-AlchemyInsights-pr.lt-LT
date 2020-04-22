---
title: "\"Office\" programų taisymas Atsiprašome, kyla laikinų serverio problemų pranešimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764125"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>"Office" programų taisymas "Atsiprašome, kyla laikinų serverio problemų" pranešimas

Jei gaunate šį pranešimą, pabandykite atlikti šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Office" programų. Peržiūrėkite [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite į **Pradėti** > **vykdyti**, tada įveskite **services.msc**. Įsitikinkite, kad visos šios tarnybos veikia:
    - Tinklo prijungtų įrenginių automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vietos žinomumas
    - Windows įvykių žurnalas

Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti. Jei kyla problemų paleidžiant tarnybą, atidarę komandinę eilutę su didesnių teisių komanda vykdykite šią komandą:

**SFC /scannow SFC /scannow SFC / scannow SFC**

Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.

Išsamesnės informacijos [ieškokite "Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai įjungiate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).