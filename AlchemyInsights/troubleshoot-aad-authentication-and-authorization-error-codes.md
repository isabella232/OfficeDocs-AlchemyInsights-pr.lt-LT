---
title: "\"Azure AD\" autentifikavimo ir įgaliojimo (\"AADSTS\") klaidų kodų trikčių šalinimas"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036510"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>"Azure AD" autentifikavimo ir įgaliojimo ("AADSTS") klaidų kodų trikčių šalinimas

Norėdami išspręsti AAD autentifikavimo ir autorizavimo klaidų kodus (AADSTS), atlikite šiuos rekomenduojamus veiksmus:

1. **"Klaidų kodų tvarkymas taikomojoje programoje"**

- " **OAuth 2.0 spec**" https://tools.ietf.org/html/rfc6749#section-5.2 , pateikiama rekomendacijų, kaip tvarkyti klaidas autentifikavimo metu naudojant klaidos atsakymo klaidos dalį.

    - **klaida**: klaidos kodo eilutė, kurią galima naudoti klasifikuojant kylančias klaidas, ir ją reikia naudoti norint reaguoti į klaidas.
    - **Klaidos** laukas turi kelias galimas reikšmes – Peržiūrėkite protokolų dokumentacijos saitus ir oauth 2,0 specifikacijas, jei reikia daugiau informacijos apie konkrečias klaidas ir kaip jas reaguoti.

- Čia pateikiamas klaidos atsakymo pavyzdys:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Peržvalgos dabartinės klaidos kodo informacija**

- Klaidų kodai ir pranešimai gali būti keičiami. Norėdami gauti naujausią informaciją, peržiūrėkite puslapį, https://login.microsoftonline.com/error kad rastumėte AADSTS klaidų aprašus, pataisymus ir kai kuriuos siūlomus sprendimo būdus.
- Taip pat galite ieškoti ir šalinti " [Aadsts" klaidų kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , išvardytus straipsnyje " [Azure AD" autentifikavimo ir autorizavimo klaidų kodai](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Gaukite pagalbos**

- [Kūrėjų palaikymo ir žinyno parinktys](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – jei jums reikia atsakymo į klausimą arba pagalbos sprendžiant problemą, kurios neapima mūsų dokumentacijoje, gali būti, kad laikas susisiekti su ekspertais pagalbos klausimais. Šiame straipsnyje pateikiami keli pasiūlymai, kaip gauti atsakymus į klausimus, kaip kurti taikomąsias programas, integruotas su "Microsoft" tapatybės platforma.








