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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727231"
---
# <a name="no-results-returned-during-content-searchexport"></a>Per turinio paiešką/eksportavimą nepateikiami jokie rezultatai

Jei kyla problemų dėl šių "elektroninės aptikimo" scenarijų:

- Turinio ieška/eksportavimas pateikia duomenų arba netikėtų duomenų
- "Udiscovery" ieška arba eksportavimas nepavyksta

Taip gali būti dėl tam tikrų atitikties saugos filtrų, kurias sąranka sukūrė konkretus administratorius ir kurios nebuvo perduotos visiems administratoriams.

Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šias problemas:

1. Prisijungimas prie saugos ir atitikties centro "PowerShell"
2. Vykdykite šiuos commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Papildomos informacijos apie atitikties saugos filtrus ieškokite [turinio ieškos teisių filtravimas](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
