---
title: Turinio ieška be rezultatų
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816856"
---
# <a name="no-results-from-content-searchexports"></a>Nėra rezultatų iš turinio ieškos / eksporto

Turinio ieškos / eksporto problemos, kurios negrąžina jokių duomenų, gali būti dėl tam tikro atitikties saugos filtro, kurį buvo sąranka konkretaus administratoriaus, o ne perduoti visiems administratoriams.

Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šią problemą:
1. Prisijungimas prie saugos ir atitikties centro "PowerShell"
2. Vykdykite šias komandas:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter organizacijos $org