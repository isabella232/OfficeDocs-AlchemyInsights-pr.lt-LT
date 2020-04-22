---
title: AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam 5.4.1 DBEB catch-all AntiSpam
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707919"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Problemos, susijusios su klaidos kodu 550 5.4.1 Perdavimo prieiga uždrausta, sprendimas

Ši problema kyla, kai [patikrinti, ar el. pašto adresas galioja siekiant išvengti bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) įvedant "Microsoft" tinklą. Pabandykite atlikti šiuos veiksmus:

1. Nustatykite, ar problema būdinga visam domenui, ar vienam el. pašto adresui:
    - Visas domenas: kartais domeną reikia sinchronizuoti; pabandykite [nustatyti domeno vidinis ir tada atgal į patikimą](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Vienas el. pašto adresas: Kartais adresą reikia sinchronizuoti; pakeisti smtp tarpinio serverio adresą ir tada jį pakeisti atgal gali padėti.
2. Nustatykite, ar problema būdinga grupei, ar viešajam aplankui. Kai kurių tipų objektams gali tekti rankiniu būdu sukurti "Azure Active Directory".

Jei jums reikia papildomos pagalbos, atidarykite palaikymo bilietą ir nurodykite problemos apimtį (įskaitant objekto, kuriam siunčiate, tipą), kad galėtume jums padėti geriau.