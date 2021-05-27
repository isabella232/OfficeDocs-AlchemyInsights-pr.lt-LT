---
title: Ediscovery trikčių šalinimas turi klaidų
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676276"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Ediscovery trikčių šalinimas turi klaidų

Kyla el. duomenų aptikimo problemų? Toliau pateikiame keletą geriausios praktikos pavyzdžių:

- Patikrinkite sulaikyto paskirstymo būseną.  Jei būsena yra **Įjungta (Laukiama)** arba **Išjungta (Laukiama)**, palaukite, kol bus baigtas sulaikytas paskirstymas.
- Sulieti el. duomenų aptikimą turi naujinimus į vieną masinę užklausą, o ne pakartotinai atnaujinti kiekvienos operacijos strategiją.
- Paleiskite Set-CaseHoldPolicy <policyname> -RetryDistribution" saugos ir atitikties centre "PowerShell". Daugiau informacijos [žr. Prisijungimas į Saugos & "PowerShell"](/powershell/exchange/connect-to-scc-powershell)atitikties centras .

Veiksmus, kaip patikrinti šiuos parametrus ir papildomą geriausią el. duomenų aptikimo švelninimo ir sprendimo praktiką, žr. [El. duomenų aptikimo sulaikymo klaidų trikčių šalinimas.](/microsoft-365/compliance/hold-distribution-errors)
Informacijos apie kitų dažnai pasitaikančių el. duomenų aptikimo trikčių diagnostiką žr. Dažniausiai pasitaikančių el. duomenų aptikimo problemų [ištyrimą, trikčių diagnostiką ir sprendimą.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
