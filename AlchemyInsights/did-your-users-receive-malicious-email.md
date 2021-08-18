---
title: Ar vartotojai gavo kenkėjiškus el. laiškus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326707"
---
# <a name="did-your-users-receive-malicious-email"></a>Ar vartotojai gavo kenkėjiškus el. laiškus?

Dabar galite pranešti apie kenkėjišką el. laišką ["Microsoft" naudodami ""Microsoft 365" sargyba portale.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Nuskaitomi pranešimai, kurie [pateikiami administratoriaus](https://security.microsoft.com/reportsubmission?viewid=admin) pateiktuose, ir toliau nurodyti rezultatai rodomi išsamios informacijos iškeliamuose meniu:

- Jeigu pristatymo metu buvo triktis dėl siuntėjo el. pašto autentifikavimo.
- Informacija apie bet kokius strategijos paspaudimus, kurie galėjo paveikti arba perrašyti pranešimo turinį.
- Dabartiniai išjungimo rezultatai, kad būtų galima peržiūrėti, ar pranešime esantys URL arba failai buvo kenkėjiški, ar ne.
- Atsiliepimai iš vertintojų

Jei aptiktas perrašymas, nuskaitymas iš naujo turėtų būti baigtas per kelias minutes. Jei nebuvo problemų dėl el. pašto autentifikavimo arba pristatymas nebuvo paveiktas dėl perrašymo, tada atsiliepimai iš vertintojų gali užtrukti iki vienos dienos.

Jei nesutiksite su galutiniu pranešimo sprendimu, URL arba failu (užblokuotu ar neužblokuotu), po dienos vėl pateikite pranešimą nuskaitymui. Tikėtina, kad dar kartą pateikus pranešimą sprendimas bus pakeistas.

Tuo tarpu galite pašalinti kenkėjiškus el. laiškus iš vartotojų aplankų Gauta vykdydami [šiame straipsnyje](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization) pateiktus nurodymus.

- Klientai, naudojantys „Microsoft“ sargybą, skirtą „Office 365“", gali:
  - Grėsmių [naršyklės naudojimas norint rasti ir panaikinti įtartinus el. laiškus](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Saitų Seifas naudojimas norint blokuoti prieigą](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) prie kenkėjiško URL
  - Vartotojų, kurie spustelėjo ir pasiekė kenkėjiškus URL, sekimas: peržiūrėkite [sukčiavimo](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)apsimetant URL ir spustelėkite sprendimo duomenis  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Automatinio [tyrimo paleidimas rankiniu būdu](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Taip pat galite apsisaugoti nuo kenkėjiškų failų ir URL vykdydami nurodymus, pateiktus [Apsauga nuo kenkėjiškų URL ir failų](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
