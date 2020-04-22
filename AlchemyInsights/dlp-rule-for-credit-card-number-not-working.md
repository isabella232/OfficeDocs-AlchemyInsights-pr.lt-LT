---
title: Neveikia Kredito kortelės numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704209"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="1f26e-102">DLP problemos su kredito kortelių numeriais</span><span class="sxs-lookup"><span data-stu-id="1f26e-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="1f26e-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="1f26e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1f26e-104">**DLP problemos su kredito kortelių numeriais**</span><span class="sxs-lookup"><span data-stu-id="1f26e-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="1f26e-105">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **kredito kortelės numeris,** kai naudojate DLP slaptos informacijos tipą O365?</span><span class="sxs-lookup"><span data-stu-id="1f26e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1f26e-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kad būtų galima suaktyvinti DLP strategiją, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="1f26e-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="1f26e-107">Pvz., **kredito kortelės strategijos,** sukonfigūruotos 85 % patikimumo lygiu, įvertinami ir turi būti aptikta, kad taisyklė būtų suaktyvinta:</span><span class="sxs-lookup"><span data-stu-id="1f26e-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="1f26e-108">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 skaitmenų, kuriuos galima formatuoti arba neformatuoti (ddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="1f26e-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="1f26e-109">**[Raštas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Labai sudėtingas ir tvirtas modelis, kuris aptinka korteles iš visų pagrindinių prekių ženklų visame pasaulyje, įskaitant "Visa", "MasterCard", "Discover Card", "JCB", "American Express", dovanų korteles ir "diner" korteles.</span><span class="sxs-lookup"><span data-stu-id="1f26e-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="1f26e-110">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Taip, Luhn kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="1f26e-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="1f26e-111">**[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP strategija yra 85% įsitikinusi, kad ji aptiko šio tipo slaptą informaciją, jei 300 simbolių atstumu:</span><span class="sxs-lookup"><span data-stu-id="1f26e-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1f26e-112">Funkcija Func_credit_card randa modelį atitinkantį turinį.</span><span class="sxs-lookup"><span data-stu-id="1f26e-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="1f26e-113">Vienas iš šių dalykų yra teisingas:</span><span class="sxs-lookup"><span data-stu-id="1f26e-113">One of the following is true:</span></span>

  - <span data-ttu-id="1f26e-114">Rastas raktinis žodis iš Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="1f26e-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="1f26e-115">Rastas raktinis žodis iš Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="1f26e-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="1f26e-116">Funkcija Func_expiration_date randa datą tinkamu datos formatu.</span><span class="sxs-lookup"><span data-stu-id="1f26e-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="1f26e-117">Kontrolinė suma praeina</span><span class="sxs-lookup"><span data-stu-id="1f26e-117">The checksum passes</span></span>

    <span data-ttu-id="1f26e-118">Pvz., šis pavyzdys būtų sukelti DLP kredito kortelės numerio strategija:</span><span class="sxs-lookup"><span data-stu-id="1f26e-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="1f26e-119">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="1f26e-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="1f26e-120">Baigiasi: 2/2009</span><span class="sxs-lookup"><span data-stu-id="1f26e-120">Expires: 2/2009</span></span>

<span data-ttu-id="1f26e-121">Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų **aptiktas kredito kortelės numeris,** ieškokite šiame šio straipsnio skyriuje: [Kokie slapti informacijos tipai ieško kredito kortelės#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="1f26e-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="1f26e-122">Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje</span><span class="sxs-lookup"><span data-stu-id="1f26e-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  