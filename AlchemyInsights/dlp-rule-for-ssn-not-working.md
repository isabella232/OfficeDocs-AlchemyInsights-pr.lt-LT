---
title: DLP taisyklė neveikia SSN
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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389441"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="3a5e9-102">DLP klausimus su socialinio draudimo numeriais</span><span class="sxs-lookup"><span data-stu-id="3a5e9-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="3a5e9-103">Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turiniu, kuriame yra **Socialinio draudimo numerį (SSN)** , kai slaptos informacijos tipą naudojant "Office 365"?</span><span class="sxs-lookup"><span data-stu-id="3a5e9-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="3a5e9-104">Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją į ką žiūri DLP strategijos.</span><span class="sxs-lookup"><span data-stu-id="3a5e9-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="3a5e9-105">Pvz., dėl SSN politikos suderintas su 85 % pasikliovimo lygmeniu, toliau yra vertinami ir turi būti nustatytas būtų sukelti taisyklė:</span><span class="sxs-lookup"><span data-stu-id="3a5e9-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3a5e9-106">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 skaitmenų, kurie gali būti formatuotą ar neformatuotą modelis</span><span class="sxs-lookup"><span data-stu-id="3a5e9-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="3a5e9-107">**[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturias funkcijas ieškokite SSNs keturių skirtingų modelių:</span><span class="sxs-lookup"><span data-stu-id="3a5e9-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="3a5e9-108">Func_ssn mano SSNs su pre-2011 ryškus formatavimas, suformatuotus brūkšnelių ar tarpų (ddd-dd-dddd ar ddd dd Andrius)</span><span class="sxs-lookup"><span data-stu-id="3a5e9-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="3a5e9-109">Func_unformatted_ssn mano SSNs su pre-2011 stiprus formatavimą, kuris yra neformatuotas devynių iš eilės einančių skaitmenų (Neringa)</span><span class="sxs-lookup"><span data-stu-id="3a5e9-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="3a5e9-110">Func_randomized_formatted_ssn randa po 2011 m. SSNs, suformatuotus brūkšnelių ar tarpų (ddd-dd-dddd ar ddd dd Andrius)</span><span class="sxs-lookup"><span data-stu-id="3a5e9-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="3a5e9-111">Func_randomized_unformatted_ssn randa po 2011 m. SSNs, kuri yra neformatuota devynių iš eilės einančių skaitmenų (pradinio ugdymo pedagogika)</span><span class="sxs-lookup"><span data-stu-id="3a5e9-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="3a5e9-112">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nėra jokių kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="3a5e9-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="3a5e9-113">**[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika yra 85 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių:</span><span class="sxs-lookup"><span data-stu-id="3a5e9-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3a5e9-114">[Func_ssn funkcija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) suranda turinį, atitinkantį modelį.</span><span class="sxs-lookup"><span data-stu-id="3a5e9-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3a5e9-115">Raktinis žodis [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) yra nustatyta.</span><span class="sxs-lookup"><span data-stu-id="3a5e9-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="3a5e9-116">Raktinių žodžių pavyzdžiai apima: *socialinės apsaugos, socialinės apsaugos #, Soc SEK, SSN* .</span><span class="sxs-lookup"><span data-stu-id="3a5e9-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="3a5e9-117">Pavyzdžiui, Šis pavyzdys paskatintų DLP SSN politikai: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="3a5e9-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="3a5e9-118">Norėdami gauti daugiau informacijos apie tai, kas yra reikalingi SSNs aptikti jūsų turinį, skaitykite kitame skyriuje šiame straipsnyje: [Kas the jautrios informacijos tipus ieškokite SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="3a5e9-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="3a5e9-119">Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3a5e9-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  