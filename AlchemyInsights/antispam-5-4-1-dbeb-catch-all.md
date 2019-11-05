---
title: AntiSpam 5.4.1 DBEB sugavimo-visi
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
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964237"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Nustatyti pristatymo problemos klaidos kodas 550 5.4.1 relės prieiga uždrausta

Ši problema kyla [tikrinant, ar el. pašto adresas galioja išvengti bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) įvesdami Office 365 tinklo. Išbandykite šiuos veiksmus:

1. Nustatyti, ar problema yra susijusi su visu domenu arba vienu el. pašto adresu:
    - Visas domenas: kartais domeną reikia sinchronizuoti; Pabandykite [nustatyti domeną į vidaus ir tada atgal į autoritetingas](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Vienas el. pašto adresas: kartais reikia sinchronizuoti adresą; keičiant SMTP tarpinio serverio adresą ir tada keičiant jį atgal gali padėti.
2. Nustatykite, ar problema yra susijusi su grupe ar viešuoju aplanku. Kai kurių objektų tipų objektai gali reikėti neautomatiniu būdu sukurti "Azure Active Directory".

Jei jums reikia papildomos pagalbos, prašome atidaryti pagalbinį bilietą ir nurodyti problemos apimtį (includidng objekto, kurį siunčiate, tipą), kad galėtume jums padėti geriau.