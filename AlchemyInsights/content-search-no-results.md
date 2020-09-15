---
title: Turinio ieškos rezultatų nėra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680655"
---
# <a name="no-results-from-content-searchexports"></a>Nėra rezultatų iš turinio ieškos/eksportavimo

Problemos dėl turinio ieškos/eksportavimo negrąžinant jokių duomenų gali būti dėl tam tikro atitikties saugos filtro, kurį nustatė konkretus administratorius, o ne visiems administratoriams.

Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šiuos veiksmus:
1. Prisijungimas prie saugos ir atitikties centro "PowerShell"
2. Vykdykite šiuos commandlets:
<br>$org = "yourdomain.com"
<br>Gauti – ComplianceSecurityFilter – organizacijos $org