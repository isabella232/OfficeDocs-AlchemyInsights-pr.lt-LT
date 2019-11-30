---
title: Aktyvinimas problema-mes negalime prisijungti dabar
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628250"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>"Office" programų taisymas "mes negalime prisijungti dabar" pranešimas

Jei gavote šį pranešimą, išbandykite toliau nurodytus veiksmus.

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Office" programėlių. Peržiūrėkite " [Office 365" URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite į **pradėti** > **vykdyti**, tada įveskite **Services. msc**. Įsitikinkite, kad visos šios tarnybos veikia:
    - Tinklo prijungtų įrenginių Automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vieta sąmoningumo
    - "Windows" įvykių žurnale

Jei viena iš šių paslaugų nepaleista, pabandykite ją paleisti. Jei turite problemų pradedant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę su didesnių teisių:

**sfc/scannow**

Po to, kai ši komanda baigia darbą, iš naujo paleiskite kompiuterį.

Išsamesnės informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau "klaida suaktyvinus Office iš Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).