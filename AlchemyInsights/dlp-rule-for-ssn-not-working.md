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
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="56c77-102">DLP problemos su socialinio draudimo numeriais</span><span class="sxs-lookup"><span data-stu-id="56c77-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="56c77-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="56c77-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="56c77-104">**DLP problemos su ŠsN**</span><span class="sxs-lookup"><span data-stu-id="56c77-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="56c77-105">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **socialinio draudimo numeris (SSN),** kai naudojate slaptą informacijos tipą "Microsoft 365"?</span><span class="sxs-lookup"><span data-stu-id="56c77-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="56c77-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, ką ieškote DLP politikoje.</span><span class="sxs-lookup"><span data-stu-id="56c77-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="56c77-107">Pvz., SSN strategijos sukonfigūruotas patikimumo lygis yra 85 %, toliau pateikiami ir turi būti aptikta taisyklė sukelti:</span><span class="sxs-lookup"><span data-stu-id="56c77-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="56c77-108">**[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 skaitmenys, kurie gali būti suformatuotame arba nesuformatuotame rašte</span><span class="sxs-lookup"><span data-stu-id="56c77-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="56c77-109">**[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos ieško SSN keturių skirtingų modelių:</span><span class="sxs-lookup"><span data-stu-id="56c77-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="56c77-110">Func_ssn randa SSN su iki 2011 m. stipriu formatu, suformatuotu brūkšneliais arba tarpais (ddd-dd-dddd or ddd ddd dddddddddddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="56c77-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="56c77-111">Func_unformatted_ssn randa SSN su iki 2011 m. stipriu formatu, kuris yra nesuformatuotas kaip devyni iš eilės skaitmenys (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="56c77-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="56c77-112">Func_randomized_formatted_ssn randa post-2011 SSN, kurie yra suformatuotas su brūkšneliais arba tarpais (ddd-dd-dddd ARBA ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="56c77-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="56c77-113">Func_randomized_unformatted_ssn randa po 2011 M. SSN, kurie yra nesuformatuoti kaip devyni iš eilės skaitmenys (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="56c77-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="56c77-114">**[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nėra kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="56c77-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="56c77-115">**[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP strategija yra 85% įsitikinusi, kad ji aptiko šio tipo slaptą informaciją, jei 300 simbolių atstumu:</span><span class="sxs-lookup"><span data-stu-id="56c77-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="56c77-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) randa šabloną atitinkantį turinį.</span><span class="sxs-lookup"><span data-stu-id="56c77-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="56c77-117">Rastas [raktinis](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) žodis iš Keyword_ssn.</span><span class="sxs-lookup"><span data-stu-id="56c77-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="56c77-118">Raktinių žodžių pavyzdžiai: *socialinė apsauga, socialinė apsauga#, Soc Sek, SSN* .</span><span class="sxs-lookup"><span data-stu-id="56c77-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="56c77-119">Pvz., šis pavyzdys būtų sukelti DLP SSN strategija: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="56c77-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="56c77-120">Jei norite gauti daugiau informacijos apie tai, ko reikia, kad SSN būtų aptikta jūsų turinį, ieškokite šiame skyriuje šiame straipsnyje: [Kas slaptos informacijos tipai ieškoti SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="56c77-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="56c77-121">Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) šiame straipsnyje</span><span class="sxs-lookup"><span data-stu-id="56c77-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  