---
title: DLP taisyklė, JAV / UK paso numeris ne darbo
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404389"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemas, susijusias su DLP - US / UK paso numeriai

Turite problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turinio turinčių a **JAV / UK paso numeris** naudojant DLP slaptos informacijos tipo O365? Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją, DLP strategijos ieško kai ji įvertinta. 
  
Pvz., per **US / UK paso numeris** politikos suderintas su 75 % pasikliovimo lygmeniu, tokios yra vertinami ir turi būti nustatyta taisyklė – sukelti 
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devyni skaičiai 
    
- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devynios iš eilės skaitmenų 
    
- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra jokių kontrolinė suma 
    
- **[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika yra 75 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių: 
    
  - Func_usa_uk_passport funkcija suranda turinį, atitinkantį modelį.
    
  - Raktinis žodis Keyword_passport yra nustatyta.
    
    Pavyzdžiui, Šis pavyzdys paskatintų už į **JAV / UK paso numeris** politika: JAV paso numeris 123456789 
    
Norėdami gauti daugiau informacijos apie tai, kas yra reikalinga JAV / UK paso numerį būtų galima aptikti turiniu, skaitykite kitame skyriuje šiame straipsnyje: [kas the jautrios informacijos tipus ieškokite JAV / UK paso numeris](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

