---
title: DLP taisyklė, skirta SSN neveikia
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004990"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemos su socialinio draudimo numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su SSN**

Ar kyla problemų dėl duomenų praradimo **prevencijos (DLP)** neveikia turiniui, kuriame yra socialinio draudimo **numeris (SSN),** kai naudojate slaptos informacijos tipą Microsoft 365? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie DLP strategiją. 
  
Pvz., SSN strategijos, sukonfigūruotos 85 % patikimumo lygiu, atveju įvertinami ir turi būti aptinkami šie taisyklės paleidimo rezultatai:
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 skaitmenys, kurie gali būti suformatuoti arba neformatuoti

- **[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos ieško SSN keturiais skirtingais modeliais:

  - Func_ssn randa SSN su iki 2011 m. stipriu formatavimu, suformatuotais brūkšneliais arba tarpais (ddd-dd-dddd OR ddd ddd dddd)

  - Func_unformatted_ssn randa SSN su iki 2011 m. stipriu formatavimu, kurie neformatuojami kaip devyni iš eilės einantys skaitmenys (dddddddddd)

  - Func_randomized_formatted_ssn randa po 2011 m. SSN, suformatuotas brūkšneliais arba tarpais (ddd-dd-dddd OR ddd ddd dddd)

  - Func_randomized_unformatted_ssn randa po 2011 m. SSN, kurie neformatuoti kaip devyni skaitmenys iš eilės (dddddddd)

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nėra "Checksum"

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP strategija yra 85 % užtikrinta, kad ji aptiko šio tipo slaptą informaciją, jei šalia 300 simbolių:

  - Funkcija [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) randa turinį, kuris atitinka šabloną.

  - Rastas [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) žodis. Raktažodžių pavyzdžiai: socialinė  *apsauga, socialinė apsauga#, Soc Sec , SSN*  . Pvz., šis pavyzdys paleis DLP SSN strategiją: **SSN: 489-36-8350**
  
Daugiau informacijos apie tai, ko reikia norint aptikti SSN jūsų turiniui, žr. šiame straipsnyje: Kas yra slaptos informacijos tipai, ieškoti [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Naudodami kitą įtaisytą slaptos informacijos tipą, informacijos apie tai, ko reikia kitiems tipams, ieškokite šiame straipsnyje: Kokio tipo [slaptos informacijos tipų ieškoti](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  