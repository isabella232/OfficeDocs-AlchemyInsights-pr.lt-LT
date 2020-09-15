---
title: "\"DLP\" taisyklės, skirtos JAV banko sąskaitos numeriui"
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679304"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>"DLP" problemos su JAV banko sąskaitų numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**"DLP" problemos su JAV banko sąskaitų numeriais**

Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **JAV banko sąskaitos numeris** , kai naudojant DLP slaptą informacijos tipą "O365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, kas yra DLP strategija, kai ji vertinama.
  
Pvz., **JAV banko sąskaitos numerio** strategija, sukonfigūruota su 85% pasikliovimo lygiu, yra vertinama ir turi būti nustatyta taisyklės, kad suaktyvintų:
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 skaitmenys

- **[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 iš eilės skaitmenys.

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra jokios kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP strategija yra 75% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:

  - Įprastas reiškinys Regex_usa_bank_account_number randa turinį, atitinkantį raštą

  - Randamas raktažodis iš Keyword_usa_Bank_Account.

    Pvz., Šis pavyzdys sukeltų **JAV banko sąskaitos numerio** strategiją: paskyros 78344011

Daugiau informacijos apie tai, ko reikia **JAV banko sąskaitos numeriui** aptikti jūsų turinyje, ieškokite šiame straipsnyje šiame straipsnyje: [kokie jautrūs informacijos tipai tinka JAV banko sąskaitos numeriui](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  