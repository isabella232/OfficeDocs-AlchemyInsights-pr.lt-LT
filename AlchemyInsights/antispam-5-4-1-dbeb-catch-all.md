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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932285"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Klaidos kodo 550 5.4.1 Perdavimo prieiga uždrausta pristatymo problemų sprendimas

Ši problema kyla [tikrinant, ar el. pašto adresas](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) galioja, kad nebūtų sugrįžta įvedant "Microsoft" tinklą. Išbandykite šiuos veiksmus:

1. Nustatykite, ar problema susijusi su visu domenu, ar vienu el. pašto adresu:
    - Visas domenas: kartais domeną reikia sinchronizuoti; pabandykite [nustatyti domeną kaip Vidinis, tada grįžkite į Patikimas](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Vienas el. pašto adresas: kartais adresą reikia sinchronizuoti; pakeisti SMTP tarpinio serverio adresą ir tada jį pakeisti atgal gali padėti.
2. Nustatykite, ar problema susijusi su grupe ar viešuoju aplanku. Kai kurių tipų objektus gali tekti sukurti rankiniu būdu naudojant "Azure Active Directory".

Jei reikia papildomos pagalbos, atidarykite palaikymo kvitą ir nurodykite problemos aprėptį (įskaitant objekto, į kurį siunčiate, tipą), kad galėtume jums padėti geriau.