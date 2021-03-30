---
title: EndPoint Manager – saugos bazinės linijos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421084"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – saugos bazinės linijos

Saugos bazinės linijos yra iš anksto sukonfigūruotos "Windows" parametrų grupės, kurios padeda taikyti saugos parametrus, rekomenduojamus atitinkamų saugos komandų. Šias bazines linijas galima tinkinti, kad būtų pateikti tik norimi parametrai ir reikšmės. Daugiau informacijos apie saugos bazines linijas žr. Saugos bazinės linijos naudojimas ["Windows 10" įrenginiams konfigūruoti "Intune".](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Šiuo metu yra šių produktų bazinės linijos:

- "Windows MDM" saugos parametrai
- "Microsoft" sargyba, skirta "EndPoint" saugos
- „Microsoft Edge“

Kiekviena bazinė informacija periodiškai atnaujinama ir išleidžiama papildomose versijose. Kiekviena versija įtraukia ir pašalina ankstesnės versijos parametrus, kad įsitikintų, jog bazinė linija atitinka dabartines rekomendacijas. "Endpoint Security" bazinės saugos konsolė leidžia palyginti skirtingas versijas, nes pakeitimai iš versijos į versiją matomi.

Patarimų, kaip efektyviausiai pakeisti bazinės linijos versiją, [žr. "Microsoft Intune" saugos bazinių linijų profilių valdymas.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Įdiegę saugos bazinę liniją, galite stebėti diegimo būseną ir peržiūrėti parametrus pagal įrenginį.

**Pastaba:** Bazinės linijos ataskaitų duomenys gali užtrukti iki 24 valandų, kad jie būtų rodomi nuo pradinio diegimo prie įrenginio ir iki 6 valandų, kad būtų galima atlikti tolesnius naujinimus. 

Dažniausia bazinės linijos parametro taikymo priežastis yra ta, kad tas pats parametras naudojamas skirtinguose profiliuose. Šį scenarijų galima ištirti konkrečiam įrenginiui pasirinkus tą įrenginį saugos bazinės linijos profilio mazge Įrenginio būsena. Daugiau informacijos [žr. Saugos bazinių duomenų konfliktų sprendimas.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)