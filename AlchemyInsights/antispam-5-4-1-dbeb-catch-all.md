---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821455"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Klaidos kodo 550 5.4.1 Perdavimo prieiga uždrausta pristatymo problemų sprendimas

Ši problema kyla [tikrinant, ar el. pašto adresas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) galioja, kad nebūtų sugrįžta įvedant "Microsoft" tinklą. Išbandykite šiuos veiksmus:

1. Nustatykite, ar problema susijusi su visu domenu, ar vienu el. pašto adresu:
    - Visas domenas: kartais domeną reikia sinchronizuoti; pabandykite [nustatyti domeną kaip Vidinis, tada grįžkite į Patikimas](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Vienas el. pašto adresas: kartais adresą reikia sinchronizuoti; pakeisti SMTP tarpinio serverio adresą ir tada jį pakeisti atgal gali padėti.
2. Nustatykite, ar problema susijusi su grupe ar viešuoju aplanku. Kai kurių tipų objektus gali tekti rankiniu būdu sukurti "Azure Active Directory".

Jei reikia papildomos pagalbos, atidarykite palaikymo kvitą ir nurodykite problemos aprėptį (įskaitant objekto, į kurį siunčiate, tipą), kad galėtume jums padėti geriau.