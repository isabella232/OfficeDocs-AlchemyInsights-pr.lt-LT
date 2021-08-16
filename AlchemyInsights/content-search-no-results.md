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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058010"
---
# <a name="no-results-from-content-searchexports"></a>Nėra rezultatų iš turinio ieškos / eksporto

Turinio ieškos / eksporto problemos, kurios negrąžina jokių duomenų, gali būti dėl tam tikro atitikties saugos filtro, kurį buvo sąranka konkretaus administratoriaus, o ne perduoti visiems administratoriams.

Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šią problemą:
1. Prisijungimas į saugos ir atitikties centro "PowerShell"
2. Vykdykite šias komandas:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter organizacijos $org