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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679449"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemos su kredito kortelių numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su kredito kortelių numeriais**

Kyla problemų, susijusių su **duomenų praradimo prevencija (DLP)** neveikia turiniui, kuriame yra **kredito kortelės numeris** , kai naudojant DLP slaptą informacijos tipą "O365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija, kad suaktyvintų DLP strategiją, kai ji vertinama. Pvz., **kredito kortelės strategijos** , sukonfigūruotos naudojant 85% pasikliautinąjį lygį, toliau pateikiami įvertinti ir turi būti aptikti taisyklės, kad būtų galima suaktyvinti:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 skaitmenų, kuriuos galima formatuoti arba nesuformatuoti (dddddddddddddddd) ir turi praeiti Luhn testą.

- **[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Labai sudėtingas ir tvirtas raštas, kuris aptinka korteles iš visų didžiųjų prekinių ženklų visame pasaulyje, įskaitant visa, MasterCard, Discover Card, JCB, American Express, dovanų korteles ir Diner korteles.

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Taip, Luhn kontrolinė suma

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP strategija yra 85% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:

  - Funkcija Func_credit_card randa turinį, atitinkantį raštą.

  - Patenkinama viena iš šių veiksmų:

  - Randamas raktažodis iš Keyword_cc_verification.

  - Randamas raktažodis iš Keyword_cc_name

  - Funkcija Func_expiration_date randa datą reikiamu datos formatu.

  - Kontrolinė suma eina

    Pvz., Šis pavyzdys turėtų suaktyvinti DLP kredito kortelės numerio strategiją:

  - Viza: 4485 3647 3952 7352
  
  - Galiojimo laikas: 2/2009

Daugiau informacijos apie tai, ko reikia **kredito kortelės numeriui** aptikti jūsų turinyje, ieškokite šiame straipsnyje šiame straipsnyje: [kas yra slaptos informacijos tipai ieškoti kredito kortelės #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  