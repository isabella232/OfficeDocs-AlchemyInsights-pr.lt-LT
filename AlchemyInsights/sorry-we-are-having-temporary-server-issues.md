---
title: "\"Office\" programėlių taisymas Atsiprašome, mes turime laikiną serverio problemos pranešimą"
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627998"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>"Office" programėlių taisymas "Atsiprašome, mes turime laikiną serverio problemos" pranešimas

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