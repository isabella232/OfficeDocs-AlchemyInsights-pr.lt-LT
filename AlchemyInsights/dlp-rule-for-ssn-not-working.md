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
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="c3ea9-102">DLP problemos su socialinio draudimo numeriais</span><span class="sxs-lookup"><span data-stu-id="c3ea9-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="c3ea9-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c3ea9-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c3ea9-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c3ea9-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="c3ea9-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c3ea9-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c3ea9-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c3ea9-109">**DLP problemos su ŠsN**</span><span class="sxs-lookup"><span data-stu-id="c3ea9-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="c3ea9-110">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **socialinio draudimo numeris (SSN),** kai naudojate slaptą informacijos tipą "Office 365"?</span><span class="sxs-lookup"><span data-stu-id="c3ea9-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="c3ea9-111">Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, ką ieškote DLP politikoje.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="c3ea9-112">Pvz., SSN strategijos sukonfigūruotas patikimumo lygis yra 85 %, toliau pateikiami ir turi būti aptikta taisyklė sukelti:</span><span class="sxs-lookup"><span data-stu-id="c3ea9-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c3ea9-113">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 skaitmenys, kurie gali būti suformatuotame arba nesuformatuotame rašte</span><span class="sxs-lookup"><span data-stu-id="c3ea9-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="c3ea9-114">**[Raštas:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Keturios funkcijos ieško SSN keturių skirtingų modelių:</span><span class="sxs-lookup"><span data-stu-id="c3ea9-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="c3ea9-115">Func_ssn randa SSN su iki 2011 m. stipriu formatu, suformatuotu brūkšneliais arba tarpais (ddd-dd-dddd or ddd ddd dddddddddddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c3ea9-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c3ea9-116">Func_unformatted_ssn randa SSN su iki 2011 m. stipriu formatu, kuris yra nesuformatuotas kaip devyni iš eilės skaitmenys (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c3ea9-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="c3ea9-117">Func_randomized_formatted_ssn randa post-2011 SSN, kurie yra suformatuotas su brūkšneliais arba tarpais (ddd-dd-dddd ARBA ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="c3ea9-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c3ea9-118">Func_randomized_unformatted_ssn randa po 2011 M. SSN, kurie yra nesuformatuoti kaip devyni iš eilės skaitmenys (dddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c3ea9-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="c3ea9-119">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, nėra kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="c3ea9-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="c3ea9-120">**[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP strategija yra 85% įsitikinusi, kad ji aptiko šio tipo slaptą informaciją, jei 300 simbolių atstumu:</span><span class="sxs-lookup"><span data-stu-id="c3ea9-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c3ea9-121">[Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) randa šabloną atitinkantį turinį.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c3ea9-122">Rastas [raktinis](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) žodis iš Keyword_ssn.</span><span class="sxs-lookup"><span data-stu-id="c3ea9-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="c3ea9-123">Raktinių žodžių pavyzdžiai: *socialinė apsauga, socialinė apsauga#, Soc Sek, SSN* .</span><span class="sxs-lookup"><span data-stu-id="c3ea9-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="c3ea9-124">Pvz., šis pavyzdys būtų sukelti DLP SSN strategija: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="c3ea9-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="c3ea9-125">Jei norite gauti daugiau informacijos apie tai, ko reikia, kad SSN būtų aptikta jūsų turinį, ieškokite šiame skyriuje šiame straipsnyje: [Kas slaptos informacijos tipai ieškoti SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="c3ea9-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="c3ea9-126">Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje</span><span class="sxs-lookup"><span data-stu-id="c3ea9-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  