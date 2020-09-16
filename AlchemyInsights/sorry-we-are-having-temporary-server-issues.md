---
title: "\"Microsoft 365\" taikomųjų programų taisymas Atsiprašome, yra laikino serverio problemų pranešimas"
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758253"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>"Microsoft 365" taikomųjų programų taisymas pranešimas "Atsiprašome, iškilo laikinų serverio problemų"

Gavę šį pranešimą, išbandykite šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Microsoft" 365 taikomųjų programų. Peržiūrėkite [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite į **pradėti**  >  **vykdyti**ir įveskite **Services. msc**. Įsitikinkite, kad visos toliau nurodytos tarnybos veikia:
    - Tinklo prijungtų įrenginių Automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vietos informacijos suvokimas
    - "Windows" įvykių registras

Jei viena iš šių tarnybų nepaleista, bandykite ją paleisti. Jei kilo problemų paleidžiant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę naudodami didesnes teises:

**sfc/scannow**

Baigę šią komandą, iš naujo paleiskite kompiuterį.

Išsamesnės informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų abonemento. Bandykite dar kartą vėliau "klaida, kai suaktyvinate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).