---
title: Aktyvinimo problema – šiuo metu negalime prisijungti
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725991"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>"Microsoft 365" taikomųjų programų taisymas pranešimas "nepavyksta prisijungti dabar"

Gavę šį pranešimą, išbandykite šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neužblokuoja interneto prieigos prie "Microsoft" 365 taikomųjų programų. Peržiūrėkite ["Microsoft" URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite į **pradėti**  >  **vykdyti**ir įveskite **Services. msc**. Įsitikinkite, kad visos toliau nurodytos tarnybos veikia:
    - Tinklo prijungtų įrenginių Automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vietos informacijos suvokimas
    - "Windows" įvykių registras

Jei viena iš šių tarnybų nepaleista, bandykite ją paleisti. Jei kilo problemų paleidžiant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę naudodami didesnes teises:

**sfc/scannow**

Baigę šią komandą, iš naujo paleiskite kompiuterį.

Išsamesnės informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų abonemento. Bandykite dar kartą vėliau "klaida, kai suaktyvinate" Office "iš" Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)".