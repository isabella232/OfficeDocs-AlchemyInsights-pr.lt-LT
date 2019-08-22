---
title: DLP taisyklė dėl kreditinės kortelės numeris, ne darbo
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529963"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemų su kredito kortelių numeriai

Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turinio su **Kredito kortelės numerį** , naudojant DLP slaptos informacijos tipo O365? Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją sukelti į DLP strategijos, kai jis yra vertinamas. Pvz., **kredito kortelės politikos** , suderintas su 85 % pasikliovimo lygmeniu, toliau yra vertinami ir turi būti nustatytas būtų sukelti taisyklė:
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 skaitmenų, kurie gali būti suformatuoti arba Neformatuotas (dddddddddddddddd) ir turi atitikti Luhn bandymo.

- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Labai sudėtingas ir tvirtą modelį, kuris aptinka korteles iš visų pagrindinių markių visame pasaulyje, įskaitant Visa, MasterCard, atrasti kortelę, JCB, American Express, dovanų kortelės, ir valgyklą korteles.

- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Taip, Luhn kontrolinė suma

- **[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika yra 85 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių:

  - Func_credit_card funkcija suranda turinį, atitinkantį modelį.

  - Tenkinama bent viena iš šių veiksmų:

  - Raktinis žodis Keyword_cc_verification yra nustatyta.

  - Raktinis žodis Keyword_cc_name yra nustatyta

  - Funkcija Func_expiration_date nustato datą tinkamą datos formatas.

  - Kontrolinės sumos eina

    Pavyzdžiui, Šis pavyzdys paskatintų DLP kreditinės kortelės numerį ir politikos:

  - Viza: 4485 3647 3952 7352
  
  - Galiojimo laikas: 2/2009

Norėdami gauti daugiau informacijos apie tai, kas reikalinga **Kreditinės kortelės numerį** , galima aptikti jūsų turinį, skaitykite kitame skyriuje šiame straipsnyje: [Kas the jautrios informacijos tipus ieškokite kreditinės kortelės #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  