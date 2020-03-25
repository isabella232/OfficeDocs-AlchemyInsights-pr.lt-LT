---
title: Neveikia NŠS DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932543"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemos su socialinio draudimo numeriais

**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą. Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus. Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.

Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus). Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais. Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.

**DLP problemos su ŠsN**

Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **socialinio draudimo numeris (SSN),** kai naudojate slaptą informacijos tipą "Office 365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, ką ieškote DLP politikoje. 
  
Pvz., SSN strategijos sukonfigūruotas patikimumo lygis yra 85 %, toliau pateikiami ir turi būti aptikta taisyklė sukelti:
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 skaitmenys, kurie gali būti suformatuotame arba nesuformatuotame rašte

- **[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos ieško SSN keturių skirtingų modelių:

  - Func_ssn randa SSN su iki 2011 m. stipriu formatu, suformatuotu brūkšneliais arba tarpais (ddd-dd-dddd or ddd ddd dddddddddddddddddddddd)

  - Func_unformatted_ssn randa SSN su iki 2011 m. stipriu formatu, kuris yra nesuformatuotas kaip devyni iš eilės skaitmenys (ddddddddddd)

  - Func_randomized_formatted_ssn randa post-2011 SSN, kurie yra suformatuotas su brūkšneliais arba tarpais (ddd-dd-dddd ARBA ddd dddd)

  - Func_randomized_unformatted_ssn randa po 2011 M. SSN, kurie yra nesuformatuoti kaip devyni iš eilės skaitmenys (dddddddddd)

- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nėra kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP strategija yra 85% įsitikinusi, kad ji aptiko šio tipo slaptą informaciją, jei 300 simbolių atstumu:

  - [Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) randa šabloną atitinkantį turinį.

  - Rastas [raktinis](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) žodis iš Keyword_ssn. Raktinių žodžių pavyzdžiai: *socialinė apsauga, socialinė apsauga#, Soc Sek, SSN* . Pvz., šis pavyzdys būtų sukelti DLP SSN strategija: **SSN: 489-36-8350**
  
Jei norite gauti daugiau informacijos apie tai, ko reikia, kad SSN būtų aptikta jūsų turinį, ieškokite šiame skyriuje šiame straipsnyje: [Kas slaptos informacijos tipai ieškoti SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje
  