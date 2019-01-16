---
title: DLP taisyklė, JAV / UK paso numeris ne darbo
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302342"
---
<span data-ttu-id="e9ff9-p101">Turite problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turinio turinčių a **JAV / UK paso numeris** naudojant DLP slaptos informacijos tipo O365? Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją, DLP strategijos ieško kai ji įvertinta.</span><span class="sxs-lookup"><span data-stu-id="e9ff9-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="e9ff9-104">Pvz., per **US / UK paso numeris** politikos suderintas su 75 % pasikliovimo lygmeniu, tokios yra vertinami ir turi būti nustatyta taisyklė – sukelti</span><span class="sxs-lookup"><span data-stu-id="e9ff9-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="e9ff9-105">**[Formatas:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devyni skaičiai</span><span class="sxs-lookup"><span data-stu-id="e9ff9-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="e9ff9-106">**[Modelis:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devynios iš eilės skaitmenų</span><span class="sxs-lookup"><span data-stu-id="e9ff9-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="e9ff9-107">**[Kontrolinė suma:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra jokių kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="e9ff9-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="e9ff9-108">**[Raiškos:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika yra 75 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių:</span><span class="sxs-lookup"><span data-stu-id="e9ff9-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e9ff9-109">Func_usa_uk_passport funkcija suranda turinį, atitinkantį modelį.</span><span class="sxs-lookup"><span data-stu-id="e9ff9-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="e9ff9-110">Raktinis žodis Keyword_passport yra nustatyta.</span><span class="sxs-lookup"><span data-stu-id="e9ff9-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="e9ff9-111">Pavyzdžiui, Šis pavyzdys paskatintų už į **JAV / UK paso numeris** politika: JAV paso numeris 123456789</span><span class="sxs-lookup"><span data-stu-id="e9ff9-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="e9ff9-112">Norėdami gauti daugiau informacijos apie tai, kas yra reikalinga JAV / UK paso numerį būtų galima aptikti turiniu, skaitykite kitame skyriuje šiame straipsnyje: [kas the jautrios informacijos tipus ieškokite JAV / UK paso numeris](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="e9ff9-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="e9ff9-113">Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e9ff9-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

