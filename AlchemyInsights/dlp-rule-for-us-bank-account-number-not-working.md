---
title: Neveikia JAV banko sąskaitos numerio DLP taisyklė
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005026"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemos su JAV banko sąskaitų numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su JAV banko sąskaitų numeriais**

Ar kyla problemų dėl duomenų **praradimo prevencijos (DLP)** neveikia turiniui, kuriame yra **JAV** banko sąskaitos numeris, kai naudojate DLP slaptos informacijos tipą "O365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, ko ieško DLP strategija, kai ji vertinama.
  
Pvz., **JAV banko sąskaitos** numerio strategijos, sukonfigūruotos su 85 % patikimumo lygiu, atveju įvertinama ir turi būti aptikta, kad taisyklė paleis:
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 skaitmenų

- **[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 skaitmenų iš eilės.

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra "Checksum"

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP strategija yra 75 % užtikrinta, kad ji aptiko šio tipo slaptą informaciją, jei šalia 300 simbolių:

  - Įprastas reiškinys Regex_usa_bank_account_number randa turinį, kuris atitinka šabloną

  - Rastas Keyword_usa_Bank_Account žodis.

    Pvz., šis pavyzdys suaktyvintų JAV banko sąskaitos numerio **strategiją:** Sąskaitos tikrinimas 78344011

Daugiau informacijos apie tai,  ko reikia, kad būtų aptiktas jūsų turinio JAV banko sąskaitos numeris, žr. šiame straipsnyje: Kas yra slaptos informacijos tipai, ieškoti [JAV banko sąskaitos numerio](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Naudodami kitą įtaisytą slaptos informacijos tipą, informacijos apie tai, ko reikia kitiems tipams, ieškokite šiame straipsnyje: Kokio tipo [slaptos informacijos tipų ieškoti](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  