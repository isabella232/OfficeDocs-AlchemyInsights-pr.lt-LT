---
title: DLP taisyklė neveikia SSN
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404425"
---
Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turiniu, kuriame yra **Socialinio draudimo numerį (SSN)** , kai slaptos informacijos tipą naudojant "Office 365"? Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją į ką žiūri DLP strategijos. 
  
Pvz., dėl SSN politikos suderintas su 85 % pasikliovimo lygmeniu, toliau yra vertinami ir turi būti nustatytas būtų sukelti taisyklė:
  
- **[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 skaitmenų, kurie gali būti formatuotą ar neformatuotą modelis 
    
- **[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturias funkcijas ieškokite SSNs keturių skirtingų modelių: 
    
  - Func_ssn mano SSNs su pre-2011 ryškus formatavimas, suformatuotus brūkšnelių ar tarpų (ddd-dd-dddd ar ddd dd Andrius)
    
  - Func_unformatted_ssn mano SSNs su pre-2011 stiprus formatavimą, kuris yra neformatuotas devynių iš eilės einančių skaitmenų (Neringa)
    
  - Func_randomized_formatted_ssn randa po 2011 m. SSNs, suformatuotus brūkšnelių ar tarpų (ddd-dd-dddd ar ddd dd Andrius)
    
  - Func_randomized_unformatted_ssn randa po 2011 m. SSNs, kuri yra neformatuota devynių iš eilės einančių skaitmenų (pradinio ugdymo pedagogika)
    
- **[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nėra jokių kontrolinė suma 
    
- **[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika yra 85 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių: 
    
  - [Func_ssn funkcija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) suranda turinį, atitinkantį modelį. 
    
  - Raktinis žodis [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) yra nustatyta. Raktinių žodžių pavyzdžiai apima: *socialinės apsaugos, socialinės apsaugos #, Soc SEK, SSN* . Pavyzdžiui, Šis pavyzdys paskatintų DLP SSN politikai: **SSN: 489-36-8350**
    
Norėdami gauti daugiau informacijos apie tai, kas yra reikalingi SSNs aptikti jūsų turinį, skaitykite kitame skyriuje šiame straipsnyje: [Kas the jautrios informacijos tipus ieškokite SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

