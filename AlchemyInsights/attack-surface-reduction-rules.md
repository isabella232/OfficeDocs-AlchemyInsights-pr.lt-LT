---
title: Atakos paviršiaus mažinimo taisyklės
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676436"
---
# <a name="attack-surface-reduction-rules"></a>Atakos paviršiaus mažinimo taisyklės

Neįtraukus failų ar aplankų, gali labai sumažėti apsauga, kurią teikia atakos paviršiaus mažinimo taisyklės. Failai, kuriuos blokavo taisyklė, leidžiami vykdyti, o ataskaita ar įvykis neįrašomi. Išimtis taikoma visoms taisyklėms, kurios leidžia išimtis.

ASR išimtys naudoja tą pačią sintaksę kaip "Microsoft" sargybos antivirusinė programa išimtys. Išsamesnės informacijos ieškokite ""Microsoft" sargybos antivirusinė programa" išimčių [konfigūravimas ir "Microsoft" sargybos antivirusinė programa.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Norėdami išvengti problemų, peržiūrėkite [Dažnai pasitaikančių klaidų, kad išvengtumėte apibrėždami išimtis](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Ne visos ASR taisyklės palaiko išimtis. Norėdami patikrinti, ar jūsų taisyklė palaiko išimtis, žr. lentelę [Atakos paviršiaus mažinimo taisyklės](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Atakos paviršiaus mažinimo taisyklės

Jūsų organizacijos atakos paviršius apima visas vietas, kuriose pažeidėjas gali pakenkti organizacijos įrenginiams ar tinklams. Atakos paviršiaus mažinimas reiškia organizacijos įrenginių ir tinklo apsaugą, todėl puolama mažiau būdų, kaip atlikti atakas. Gali padėti "Microsoft" sargybos galinio punkto atakos paviršiaus mažinimo taisyklių konfigūravimas.

Daugiau informacijos rasite:

- [Susieti ASR taisyklės GUID pavadinimą](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR taisyklių reikalavimai:
    - [Windows 10 Pro 1709 arba naujesnė versija](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise 1709 arba naujesnė versija](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, version 1803 (Semi-Annual Channel) or later](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Tinkamos taikyti išimties identifikas

1. "Microsoft-Windows-"Windows" sargyba" žurnale ieškokite įvykio ID 1121 arba 1122.

1. Įvertinkite blokavimo scenarijų ir kontekstą ir patvirtinkite, kad šis scenarijus turi būti atblokuotas.

1. Įvykio išsamioje dalyje perskaitykite reikšmę Kelias, kuri yra reikšmę, kuri apibrėžia išimtį.
    - Padarykite, kad išimtis būtų kuo griežtesnė.
    - Prireikus pritaikykite pakaitos simbolį (pvz., pakeiskite vartotojo kintamąjį).

1. Taikyti išimtį pagal savo diegimo poreikius. Daugiau informacijos žr. [Atakos paviršiaus mažinimo taisyklių tinkinimas.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Išimtis nepaiso

1. Nustatykite, ar taisyklė palaiko išimtis. Daugiau informacijos žr. [Atakos paviršiaus mažinimo taisyklės](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Peržiūrėkite taikomas išimtis ir patikrinkite naudodami rašybos klaidų arba klaidingai interpretuotos pakaitos simbolių įvykio duomenis. Daugiau informacijos žr. [Palaikomi išimčių tipai](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. jei taisyklės poveikis per didelis, apsvarstykite galimybę perkelti taisyklę (atgal) į audito režimą, kad būtų galima atlikti tolesnį tikrinimą. Daugiau informacijos žr. [Tikrinimas, kaip "Microsoft" sargyba galinių punktų funkcijoms veikia audito režimu](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Norėdami atidaryti palaikymo atvejį, rinkite palaikymo duomenis naudodami šią komandą:
    
   ** MDEClientAnalyzer.cmd -v**

    Daugiau informacijos žr. ["Microsoft" sargybos galinių punktų parengimo įrenginių problemos.](issues-with-onboarding-machines.md)
