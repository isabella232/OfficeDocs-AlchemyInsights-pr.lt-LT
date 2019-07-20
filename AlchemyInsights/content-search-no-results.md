---
title: Turinio paieška jokių rezultatų
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800474"
---
# <a name="no-results-from-content-searchexports"></a>Jokių rezultatų iš turinio paieškos/eksportas

Problemos su turinio paieškos/eksporto negrįžta duomenis gali būti dėl tam tikrų atitikties saugos filtrą, kuris buvo setup iš konkrečių Admin ir nėra perduoti visi administratorių.

Norėdami išspręsti šią problemą, patikrinkite, ar yra bet atitikties saugos filtrus, kurie gali kelti tai:
1. Prisijungti prie saugos ir atitikties užtikrinimo centre "PowerShell"
2. Vykdykite ir toliau "commandlet" komandas.
<br>$org = "yourdomain.com"
<br>Gauti ComplianceSecurityFilter-organizacijos $org