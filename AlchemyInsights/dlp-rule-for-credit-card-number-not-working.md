---
title: Neveikia kredito kortelės numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005098"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemos su kredito kortelių numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su kredito kortelių numeriais**

Ar kyla problemų dėl duomenų  **praradimo prevencijos (DLP)** neveikia turiniui, kuriame yra kredito kortelės numeris, kai naudojate DLP slaptos informacijos tipą "O365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikiamos informacijos, kad būtų suaktyvinta DLP strategija, kai ji įvertinama. Pvz., kredito **kortelės strategijos,** sukonfigūruotos 85 % patikimumo lygiu, atveju įvertinami ir turi būti aptinkami šie taisyklės paleidimo rezultatai:
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 skaitmenų, kurie gali būti suformatuoti arba neformatuoti (dddddddddddddd) ir turi išlaikyti Luhn testą.

- **[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Labai sudėtingas ir patikimas modelis, kuris aptinka korteles iš visų pagrindinių prekių ženklų visame pasaulyje, įskaitant "Visa", "MasterCard", "Discover Card", JCB, "American Express", dovanų korteles ir diner korteles.

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Taip, Luhn checksum

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP strategija yra 85 % užtikrinta, kad ji aptiko šio tipo slaptą informaciją, jei šalia 300 simbolių:

  - Funkcija Func_credit_card randa turinį, kuris atitinka šabloną.

  - Teisingas vienas iš šių sąlygų:

  - Rastas Keyword_cc_verification žodis.

  - Rastas Keyword_cc_name žodis

  - Funkcija Func_expiration_date randa datą tinkamu datos formatu.

  - Pereina čekis

    Pvz., šis pavyzdys paleis DLP kredito kortelės numerio strategiją:

  - Visa: 4485 3647 3952 7352
  
  - Baigiasi: 2009-02-02

Daugiau informacijos apie tai,  ko reikia norint aptikti jūsų turinio kredito kortelės numerį, žr. šiame straipsnyje: Kas yra slaptos informacijos tipai, [ieškoti kredito kortelės#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Naudodami kitą įtaisytą slaptos informacijos tipą, informacijos apie tai, ko reikia kitiems tipams, ieškokite šiame straipsnyje: Kokio tipo [slaptos informacijos tipų ieškoti](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  