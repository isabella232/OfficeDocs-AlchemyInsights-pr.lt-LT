---
title: Neveikia NŠS DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507378"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemos su socialinio draudimo numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su ŠsN**

Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **socialinio draudimo numeris (SSN),** kai naudojate slaptą informacijos tipą "Microsoft 365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, ką ieškote DLP politikoje. 
  
Pvz., SSN strategijos sukonfigūruotas patikimumo lygis yra 85 %, toliau pateikiami ir turi būti aptikta taisyklė sukelti:
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 skaitmenys, kurie gali būti suformatuotame arba nesuformatuotame rašte

- **[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos ieško SSN keturių skirtingų modelių:

  - Func_ssn randa SSN su iki 2011 m. stipriu formatu, suformatuotu brūkšneliais arba tarpais (ddd-dd-dddd or ddd ddd dddddddddddddddddddddd)

  - Func_unformatted_ssn randa SSN su iki 2011 m. stipriu formatu, kuris yra nesuformatuotas kaip devyni iš eilės skaitmenys (ddddddddddd)

  - Func_randomized_formatted_ssn randa post-2011 SSN, kurie yra suformatuotas su brūkšneliais arba tarpais (ddd-dd-dddd ARBA ddd dddd)

  - Func_randomized_unformatted_ssn randa po 2011 M. SSN, kurie yra nesuformatuoti kaip devyni iš eilės skaitmenys (dddddddddd)

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nėra kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP strategija yra 85% įsitikinusi, kad ji aptiko šio tipo slaptą informaciją, jei 300 simbolių atstumu:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) randa šabloną atitinkantį turinį.

  - Rastas [raktinis](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) žodis iš Keyword_ssn. Raktinių žodžių pavyzdžiai: *socialinė apsauga, socialinė apsauga#, Soc Sek, SSN* . Pvz., šis pavyzdys būtų sukelti DLP SSN strategija: **SSN: 489-36-8350**
  
Jei norite gauti daugiau informacijos apie tai, ko reikia, kad SSN būtų aptikta jūsų turinį, ieškokite šiame skyriuje šiame straipsnyje: [Kas slaptos informacijos tipai ieškoti SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) šiame straipsnyje
  