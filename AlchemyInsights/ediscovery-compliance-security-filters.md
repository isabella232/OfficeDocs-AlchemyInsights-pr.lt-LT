---
title: Turinio ieškos / eksportavimo metu negrąžinti jokie rezultatai
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101274"
---
# <a name="no-results-returned-during-content-searchexport"></a>Turinio ieškos / eksportavimo metu negrąžinti jokie rezultatai

Jei kyla problemų dėl šių el. duomenų aptikimo scenarijų:

- Turinio ieška / eksportavimas negrąžina jokių duomenų arba netikėtų duomenų
- El. duomenų aptikimo ieška arba eksportavimas nepavyksta

Taip gali būti dėl tam tikrų atitikties saugos filtrų, kurie buvo nustatyti konkretaus administratoriaus ir kurie nebuvo perduoti visiems administratoriams.

Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šias problemas:

1. Prisijungimas į saugos ir atitikties centro "PowerShell"
2. Vykdykite šias komandas:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Papildomos informacijos apie atitikties saugos filtrus žr. [Turinio ieškos teisių filtravimas](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
