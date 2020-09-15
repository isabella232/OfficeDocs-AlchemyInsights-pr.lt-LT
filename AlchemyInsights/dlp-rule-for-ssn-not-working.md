---
title: Neveikia SSN taisyklė
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679377"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemos su socialinio draudimo numeriais

**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).

**DLP problemos su "SNS"**

Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** , naudojamo turiniui, kuriame yra **socialinio draudimo numeris (SSN)** , naudojant slaptos informacijos tipą programoje "Microsoft 365"? Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, kas ieško DLP strategijos. 
  
Pvz., jei taikoma SSN strategija, kurios patikimumo lygis yra 85%, toliau pateikiami įvertinti ir turi būti aptikti taisyklės, kad būtų galima suaktyvinti:
  
- **[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 skaitmenys, kurie gali būti suformatuotas arba Neformatuotas raštas

- **[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos – ieškoti kelių skirtingų modelių.

  - Func_ssn randa "SNS" su "2011" griežtu formatavimu, suformatuotu brūkšnelių ar tarpų (DDD-DD-dddd arba DDD DD dddd)

  - Func_unformatted_ssn randa "SNS" su "2011" griežtu formatavimu, kuris yra nesuformatuotas kaip devyni iš eilės einantys skaitmenys (ddddddddd)

  - Func_randomized_formatted_ssn randa "2011", kurie yra formatuoti naudojant brūkšnelių ar tarpų (DDD-DD-dddd arba DDD DD dddd).

  - Func_randomized_unformatted_ssn randa post-2011 s, kurie yra nesuformatuoti kaip devyni skaitmenys iš eilės (ddddddddd)

- **[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nėra jokios kontrolinės sumos

- **[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP strategija yra 85% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) randa turinį, atitinkantį raštą.

  - Randamas raktažodis iš [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Raktažodžių pavyzdžiai:  *socialinis saugumas, socialinis saugumas #, SOC SEC, SSN*  . Pvz., Šis pavyzdys sukeltų DLP "SSN" strategiją: " **SSN": 489-36-8350**
  
Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų galima aptikti SSNs, ieškokite šiame straipsnyje šiame straipsnyje: kas yra [slaptos informacijos tipai ieškos SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  