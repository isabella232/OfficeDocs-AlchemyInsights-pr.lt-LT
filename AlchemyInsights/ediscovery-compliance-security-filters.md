---
title: Per turinio paiešką/eksportavimą nepateikiami jokie rezultatai
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678681"
---
# <a name="no-results-returned-during-content-searchexport"></a>Per turinio paiešką/eksportavimą nepateikiami jokie rezultatai

Jei kyla problemų dėl šių "elektroninės aptikimo" scenarijų:

- Turinio ieška/eksportavimas pateikia duomenų arba netikėtų duomenų
- "Udiscovery" ieška arba eksportavimas nepavyksta

Taip gali nutikti dėl tam tikrų atitikties saugos filtrų, kurie buvo sukonfigūruoti konkrečiame administratoriaus ir nebuvo perduoti visiems administratoriams.

Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šias problemas:

1. Prisijungimas prie saugos ir atitikties centro "PowerShell"
2. Vykdykite šiuos commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Papildomos informacijos apie atitikties saugos filtrus ieškokite [turinio ieškos teisių filtravimas](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
