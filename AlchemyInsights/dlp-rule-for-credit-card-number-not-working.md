---
title: Neveikia Kredito kortelės numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704209"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemos su kredito kortelių numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

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
  