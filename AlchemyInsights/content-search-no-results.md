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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516787"
---
# <a name="no-results-from-content-searchexports"></a>Jokių rezultatų iš turinio paieškos/eksportas

Problemos su turinio paieškos/eksporto negrįžta duomenis gali būti dėl tam tikrų atitikties saugos filtrą, kuris buvo setup iš konkrečių Admin ir nėra perduoti visi administratorių.

Norėdami išspręsti šią problemą, patikrinkite, ar yra bet atitikties saugos filtrus, kurie gali kelti tai:
1. Prisijungti prie saugos ir atitikties užtikrinimo centre "PowerShell"
2. Vykdykite ir toliau "commandlet" komandas.
<br>$org = "yourdomain.com"
<br>Gauti ComplianceSecurityFilter-organizacijos $org