---
title: Vartotojas gauna klaidos AADSTS7000112 "Yammer" yra išjungtas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198054"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Vartotojas gauna klaidos AADSTS7000112 "Yammer" yra išjungtas

Jei gaunate klaidos pranešimą "AADSTS7000112: programa"00000005-0000-0ff1-ce00-00000000000"("Yammer") yra išjungta", problema yra su tarnybos pagrindinė per Azure AD. Administratorius galėjo išjungti pagrindinę tarnybą, kad užblokuotų prieigą prie "Yammer".

Tarnybos pagrindinės sistemos išjungimas nerekomenduojamas ir gali sukelti papildomų problemų. Daugiau informacijos apie palaikomą vartotojo prieigos prie "Yammer" blokavimo metodą rasite ["Yammer" prieigos išjungimas "Microsoft 365" vartotojams](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Norėdami išspręsti šią problemą Azure portalas ir atkurti vartotojo prieigą prie "Yammer":

1.  Atidarykite "Azure Active Directory" puslapį ir kairiojoje naršymo srityje dalyje **Tvarkyti** pasirinkite **Įmonės taikomosios programos.**
3.  Ieškos lauke įveskite **"Office 365" "Yammer"** ir pasirinkite programos pavadinimą, kad atidarytumėte parametrus.
4.  Kairiojoje naršymo srityje dalyje **Tvarkyti** pasirinkite **Ypatybės.**
5.  Nustatykite **reikšmę Įgalinta vartotojams prisijungti?** **Yes** **Save**
6.  Vėl prisijunkite prie "Yammer". Gali reikėti išvalyti slapukus.

Arba paleiskite "PowerShell" komandas, kad nustatytumėte reikšmę. Jei reikia daugiau informacijos, [peržiūrėkite klaidos pranešimą "Atsiprašome, bet kyla problemų prisijungiant prie jūsų", kai "Office 365" spustelite "Yammer" plytelę](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 