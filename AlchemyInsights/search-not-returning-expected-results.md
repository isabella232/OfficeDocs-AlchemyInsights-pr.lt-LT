---
title: 1491-paieškos ne grįžtant laukiami rezultatai
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709235"
---
# <a name="content-search-not-returning-expected-results"></a>Turinio ieška nepateikia numatomų rezultatų

Kai vykdote turinio ieškas iš "Microsoft 365" saugos & atitikties centro, galite gauti netikėtų ieškos rezultatų. Apsvarstykite šiuos dalykus, kurie gali turėti įtakos ieškos rezultatams:

- **Turinio vietos ir paieškos sąlygos**: įsitikinkite, kad pasirinkote tinkamas turinio vietas ir paieškos sąlygas. Jei vykdėte didelę paiešką (su daugeliu vietų), apsvarstykite galimybę ją skaidyti į kelias paieškas.

- **Iš dalies indeksuoti elementai:** [iš dalies indeksuoti pašto](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) dėžučių elementai įtraukiami į įvertintus ieškos rezultatus. Tačiau iš dalies indeksuoti elementai iš "SharePoint" ir "OneDrive" svetainių neįtraukiami į ieškos įvertinimą.

- **Ieškos triktys**: ieškodami daug pašto dėžučių (daugiau nei 100 000 pašto dėžučių), galite gauti ieškos klaidų, naudodami klaidų kodus, pvz., CS008-009 ir CS012-002). Tokiu atveju bandykite ieškoti tik nepavyko turinio vietose. Daugiau informacijos rasite [šiame straipsnyje.](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)
