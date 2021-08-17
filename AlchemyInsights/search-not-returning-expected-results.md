---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052718"
---
# <a name="content-search-not-returning-expected-results"></a>Turinio ieška negrąžina laukiamų rezultatų

Vykdydami turinio ieškas iš Microsoft 365 saugos & centro, galite gauti netikėtų ieškos rezultatų. Apsvarstykite šiuos dalykus, kurie gali turėti įtakos ieškos rezultatams:

- **Turinio vietos ir ieškos sąlygos:** įsitikinkite, kad pasirinkote tinkamas turinio vietas ir ieškos sąlygas. Jei vyko didelė ieška (su daugeliu vietų), apsvarstykite galimybę ją padalyti į kelias ieškas.

- **Iš dalies indeksuoti elementai**:  [Iš dalies indeksuoti](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) pašto dėžučių elementai įtraukiami į numatomą ieškos rezultatą. Tačiau iš dalies indeksuoti elementai iš SharePoint "OneDrive" nėra įtraukti į ieškos įvertinimą.

- Ieškos klaidos: ieškodami daug pašto dėžučių (daugiau nei 100 000 pašto dėžučių), galite gauti ieškos klaidų su klaidų **kodais,** pvz., CS008-009 ir CS012-002). Tokiu atveju bandykite dar kartą ieškoti tik nepavykusių turinio vietų. Daugiau  [informacijos žr.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) šiame straipsnyje.
