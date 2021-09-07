---
title: „EndPoint Manager“ - saugos bazinės konfigūracijos
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
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923562"
---
# <a name="endpoint-manager---security-baselines"></a>„EndPoint Manager“ - saugos bazinės konfigūracijos

Saugos bazinės konfigūracijos yra iš anksto sukonfigūruotos „Windows“ parametrų grupės, kurios padeda pritaikyti saugos parametrus, kuriuos rekomenduoja atitinkamos saugos komandos. Šias bazines konfigūracijas galima tinkinti, kad būtų pateikti tik norimi parametrai ir vertės. Norėdami gauti daugiau informacijos apie saugos bazines konfigūracijas, žr. [Saugos bazinių konfigūracijų naudojimas konfigūruojant „Windows 10“ įrenginius „Intune“](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Šiuo metu yra šių produktų bazinės konfigūracijos:

- „Windows MDM“ saugos parametrai
- „Microsoft“ sargyba, skirta pabaigos taško saugai
- „Microsoft Edge“

Kiekviena bazinė konfigūracija yra periodiškai atnaujinama ir išleidžiama palaipsniui. Kiekviena versija įtraukia ir / arba pašalina ankstesnės versijos parametrus, kad būtų užtikrinta, jog bazinė konfigūracija atitinka dabartinius nurodymus. Saugos bazinių konfigūracijų konsolė pabaigos taško saugoje leidžia palyginti skirtingas versijas, matant pakeitimus iš vienos versijos į kitą.

Dėl nurodymų, kaip efektyviausiai keisti diegiamą bazinės konfigūracijos versiją, žr. [ „Microsoft Intune“ saugos bazinės konfigūracijos tvarkymas](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Pritaikę saugos bazinę konfigūraciją, galite stebėti diegimo būseną ir peržiūrėti parametrus kiekviename įrenginyje.

Kadangi saugos bazinėse linijose yra daug parametrų, svarbu peržiūrėti konfigūracijos pakeitimus ir atlikti testavimą, kad visi parametrai būtų tinkami jūsų įrenginiams ir verslo poreikiams.

**Pastaba:** bazinių konfigūracijų ataskaitų duomenys gali užtrukti iki 24 valandų, kol bus rodomos po pradinio diegimo įrenginyje, o iki tolesnių naujinimų - iki 6 valandų. 

Dažniausia bazinės konfigūracijos parametro netaikymo priežastis yra ta, kad tas pats parametras naudojamas kitame profilyje. Šį scenarijų galima ištirti konkrečiam įrenginiui, pasirinkus tą įrenginį iš įrenginio būsenos mazgo saugos bazinės konfigūracijos profilyje. Daugiau informacijos žr. [Saugos bazinių konfigūracijų konfliktų sprendimas](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).