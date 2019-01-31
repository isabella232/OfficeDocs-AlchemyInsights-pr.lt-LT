---
title: DLP taisyklė neveikia SSN
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657367"
---
<span data-ttu-id="dd3ad-p101">Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turiniu, kuriame yra **Socialinio draudimo numerį (SSN)** , kai slaptos informacijos tipą naudojant "Office 365"? Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją į ką žiūri DLP strategijos.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="dd3ad-104">Pvz., dėl SSN politikos suderintas su 85 % pasikliovimo lygmeniu, toliau yra vertinami ir turi būti nustatytas būtų sukelti taisyklė:</span><span class="sxs-lookup"><span data-stu-id="dd3ad-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="dd3ad-105">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 skaitmenų, kurie gali būti formatuotą ar neformatuotą modelis</span><span class="sxs-lookup"><span data-stu-id="dd3ad-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="dd3ad-106">**[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturias funkcijas ieškokite SSNs keturių skirtingų modelių:</span><span class="sxs-lookup"><span data-stu-id="dd3ad-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="dd3ad-107">Func_ssn mano SSNs su pre-2011 ryškus formatavimas, suformatuotus brūkšnelių ar tarpų (ddd-dd-dddd ar ddd dd Andrius)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="dd3ad-108">Func_unformatted_ssn mano SSNs su pre-2011 stiprus formatavimą, kuris yra neformatuotas devynių iš eilės einančių skaitmenų (Neringa)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="dd3ad-109">Func_randomized_formatted_ssn randa po 2011 m. SSNs, suformatuotus brūkšnelių ar tarpų (ddd-dd-dddd ar ddd dd Andrius)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="dd3ad-110">Func_randomized_unformatted_ssn randa po 2011 m. SSNs, kuri yra neformatuota devynių iš eilės einančių skaitmenų (pradinio ugdymo pedagogika)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="dd3ad-111">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nėra jokių kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="dd3ad-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="dd3ad-112">**[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika yra 85 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių:</span><span class="sxs-lookup"><span data-stu-id="dd3ad-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="dd3ad-113">[Func_ssn funkcija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) suranda turinį, atitinkantį modelį.</span><span class="sxs-lookup"><span data-stu-id="dd3ad-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="dd3ad-p102">Raktinis žodis [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) yra nustatyta. Raktinių žodžių pavyzdžiai apima: *socialinės apsaugos, socialinės apsaugos #, Soc SEK, SSN* . Pavyzdžiui, Šis pavyzdys paskatintų DLP SSN politikai: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="dd3ad-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="dd3ad-117">Norėdami gauti daugiau informacijos apie tai, kas yra reikalingi SSNs aptikti jūsų turinį, skaitykite kitame skyriuje šiame straipsnyje: [Kas the jautrios informacijos tipus ieškokite SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="dd3ad-118">Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dd3ad-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

