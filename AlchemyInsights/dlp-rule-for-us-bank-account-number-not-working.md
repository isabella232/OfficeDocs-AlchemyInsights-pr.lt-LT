---
title: Neveikia JAV banko sąskaitos numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932553"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemos su JAV banko sąskaitų numeriais

**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą. Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus. Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.

Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus). Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais. Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.

**DLP problemos su JAV banko sąskaitų numeriais**

Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **JAV banko sąskaitos numeris,** kai naudojate DLP slaptos informacijos tipą O365? Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kurios ieškote, kai ji vertinama.
  
Pvz., **JAV banko sąskaitos numerio** strategija, sukonfigūruota 85 % patikimumo lygiu, įvertinami ir turi būti aptikta, kad taisyklė būtų suaktyvinta:
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 skaitmenų

- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 skaitmenų iš eilės.

- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP strategija yra 75% įsitikinusi, kad ji aptiko tokio tipo slaptą informaciją, jei 300 simbolių atstumu:

  - Paprastoji išraiška Regex_usa_bank_account_number randa šabloną atitinkantį turinį

  - Rastas raktinis žodis iš Keyword_usa_Bank_Account.

    Pvz., jav **banko sąskaitos numerio** strategijos suaktyvinamas šis pavyzdys: tikrinimo sąskaita 78344011

Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų **aptiktas JAV banko sąskaitos numeris,** ieškokite šiame šio straipsnio skyriuje: [Kokie slaptos informacijos tipai ieško JAV banko sąskaitos numerio](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje
  