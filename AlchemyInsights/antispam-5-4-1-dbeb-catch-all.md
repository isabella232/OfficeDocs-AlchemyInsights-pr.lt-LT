---
title: AntiSpam 5.4.1 DBEB catch-All
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717369"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Problemų, susijusių su klaidos kodu 550 5.4.1 Relay prieiga uždrausta, šalinimas

Ši problema kyla [tikrinant, ar el. pašto adresas galioja, kad būtų išvengta "bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) " įvedant "Microsoft" tinklą. Išbandykite šiuos veiksmus:

1. Nustatykite, ar problema būdinga visam domenui, ar vienam elektroninio pašto adresui:
    - Visas domenas: kartais domeną reikia sinchronizuoti; Pabandykite [nustatyti domeną kaip vidinį ir grįžti į patikimą](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Vienas elektroninio pašto adresas: kartais adresą reikia sinchronizuoti; pakeitus SMTP tarpinio serverio adresą ir pakeitus jį atgal, gali padėti.
2. Nustatykite, ar problema būdinga grupei ar viešajam aplankui. Kai kurių objektų tipų objektams gali reikėti rankiniu būdu sukurti "Azure Active Directory".

Jei reikia papildomos pagalbos, atidarykite palaikymo bilietą ir nurodykite problemos aprėptį (įskaitant objekto, kurį siunčiate, tipą), kad galėtume jums padėti geriau.