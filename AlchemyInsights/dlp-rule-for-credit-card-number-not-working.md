---
title: Neveikia Kredito kortelės numerio DLP taisyklė
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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977206"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemos su kredito kortelių numeriais

**Svarbu:** šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos išliktų labai pasiekiamos – daugiau informacijos rasite ["SharePoint Online" laikinieji funkcijų koregavimai.](https://aka.ms/ODSPAdjustments)

**DLP problemos su kredito kortelių numeriais**

Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **kredito kortelės numeris,** kai naudojate DLP slaptos informacijos tipą O365? Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kad būtų galima suaktyvinti DLP strategiją, kai ji vertinama. Pvz., **kredito kortelės strategijos,** sukonfigūruotos 85 % patikimumo lygiu, įvertinami ir turi būti aptikta, kad taisyklė būtų suaktyvinta:
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 skaitmenų, kuriuos galima formatuoti arba neformatuoti (ddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

- **[Raštas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Labai sudėtingas ir tvirtas modelis, kuris aptinka korteles iš visų pagrindinių prekių ženklų visame pasaulyje, įskaitant "Visa", "MasterCard", "Discover Card", "JCB", "American Express", dovanų korteles ir "diner" korteles.

- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Taip, Luhn kontrolinė suma

- **[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP strategija yra 85% įsitikinusi, kad ji aptiko šio tipo slaptą informaciją, jei 300 simbolių atstumu:

  - Funkcija Func_credit_card randa modelį atitinkantį turinį.

  - Vienas iš šių dalykų yra teisingas:

  - Rastas raktinis žodis iš Keyword_cc_verification.

  - Rastas raktinis žodis iš Keyword_cc_name

  - Funkcija Func_expiration_date randa datą tinkamu datos formatu.

  - Kontrolinė suma praeina

    Pvz., šis pavyzdys būtų sukelti DLP kredito kortelės numerio strategija:

  - Viza: 4485 3647 3952 7352
  
  - Baigiasi: 2/2009

Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų **aptiktas kredito kortelės numeris,** ieškokite šiame šio straipsnio skyriuje: [Kokie slapti informacijos tipai ieško kredito kortelės#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje
  