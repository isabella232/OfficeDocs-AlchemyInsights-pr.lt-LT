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
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4c698-102">DLP problemos su socialinio draudimo numeriais</span><span class="sxs-lookup"><span data-stu-id="4c698-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4c698-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4c698-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4c698-104">**DLP problemos su "SNS"**</span><span class="sxs-lookup"><span data-stu-id="4c698-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4c698-105">Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** , naudojamo turiniui, kuriame yra **socialinio draudimo numeris (SSN)** , naudojant slaptos informacijos tipą programoje "Microsoft 365"?</span><span class="sxs-lookup"><span data-stu-id="4c698-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="4c698-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, kas ieško DLP strategijos.</span><span class="sxs-lookup"><span data-stu-id="4c698-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4c698-107">Pvz., jei taikoma SSN strategija, kurios patikimumo lygis yra 85%, toliau pateikiami įvertinti ir turi būti aptikti taisyklės, kad būtų galima suaktyvinti:</span><span class="sxs-lookup"><span data-stu-id="4c698-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4c698-108">**[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 skaitmenys, kurie gali būti suformatuotas arba Neformatuotas raštas</span><span class="sxs-lookup"><span data-stu-id="4c698-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4c698-109">**[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos – ieškoti kelių skirtingų modelių.</span><span class="sxs-lookup"><span data-stu-id="4c698-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4c698-110">Func_ssn randa "SNS" su "2011" griežtu formatavimu, suformatuotu brūkšnelių ar tarpų (DDD-DD-dddd arba DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="4c698-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4c698-111">Func_unformatted_ssn randa "SNS" su "2011" griežtu formatavimu, kuris yra nesuformatuotas kaip devyni iš eilės einantys skaitmenys (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4c698-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4c698-112">Func_randomized_formatted_ssn randa "2011", kurie yra formatuoti naudojant brūkšnelių ar tarpų (DDD-DD-dddd arba DDD DD dddd).</span><span class="sxs-lookup"><span data-stu-id="4c698-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4c698-113">Func_randomized_unformatted_ssn randa post-2011 s, kurie yra nesuformatuoti kaip devyni skaitmenys iš eilės (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4c698-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4c698-114">**[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, nėra jokios kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="4c698-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4c698-115">**[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP strategija yra 85% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:</span><span class="sxs-lookup"><span data-stu-id="4c698-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4c698-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) randa turinį, atitinkantį raštą.</span><span class="sxs-lookup"><span data-stu-id="4c698-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4c698-117">Randamas raktažodis iš [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="4c698-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="4c698-118">Raktažodžių pavyzdžiai:  *socialinis saugumas, socialinis saugumas #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="4c698-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4c698-119">Pvz., Šis pavyzdys sukeltų DLP "SSN" strategiją: " **SSN": 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4c698-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4c698-120">Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų galima aptikti SSNs, ieškokite šiame straipsnyje šiame straipsnyje: kas yra [slaptos informacijos tipai ieškos SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4c698-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4c698-121">Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4c698-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  