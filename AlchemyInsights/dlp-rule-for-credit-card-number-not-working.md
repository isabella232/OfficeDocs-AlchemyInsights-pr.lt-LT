---
title: DLP taisyklė dėl kreditinės kortelės numeris, ne darbo
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529963"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="be247-102">DLP problemų su kredito kortelių numeriai</span><span class="sxs-lookup"><span data-stu-id="be247-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="be247-103">Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turinio su **Kredito kortelės numerį** , naudojant DLP slaptos informacijos tipo O365?</span><span class="sxs-lookup"><span data-stu-id="be247-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="be247-104">Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją sukelti į DLP strategijos, kai jis yra vertinamas.</span><span class="sxs-lookup"><span data-stu-id="be247-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="be247-105">Pvz., **kredito kortelės politikos** , suderintas su 85 % pasikliovimo lygmeniu, toliau yra vertinami ir turi būti nustatytas būtų sukelti taisyklė:</span><span class="sxs-lookup"><span data-stu-id="be247-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="be247-106">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 skaitmenų, kurie gali būti suformatuoti arba Neformatuotas (dddddddddddddddd) ir turi atitikti Luhn bandymo.</span><span class="sxs-lookup"><span data-stu-id="be247-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="be247-107">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Labai sudėtingas ir tvirtą modelį, kuris aptinka korteles iš visų pagrindinių markių visame pasaulyje, įskaitant Visa, MasterCard, atrasti kortelę, JCB, American Express, dovanų kortelės, ir valgyklą korteles.</span><span class="sxs-lookup"><span data-stu-id="be247-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="be247-108">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Taip, Luhn kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="be247-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="be247-109">**[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika yra 85 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių:</span><span class="sxs-lookup"><span data-stu-id="be247-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="be247-110">Func_credit_card funkcija suranda turinį, atitinkantį modelį.</span><span class="sxs-lookup"><span data-stu-id="be247-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="be247-111">Tenkinama bent viena iš šių veiksmų:</span><span class="sxs-lookup"><span data-stu-id="be247-111">One of the following is true:</span></span>

  - <span data-ttu-id="be247-112">Raktinis žodis Keyword_cc_verification yra nustatyta.</span><span class="sxs-lookup"><span data-stu-id="be247-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="be247-113">Raktinis žodis Keyword_cc_name yra nustatyta</span><span class="sxs-lookup"><span data-stu-id="be247-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="be247-114">Funkcija Func_expiration_date nustato datą tinkamą datos formatas.</span><span class="sxs-lookup"><span data-stu-id="be247-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="be247-115">Kontrolinės sumos eina</span><span class="sxs-lookup"><span data-stu-id="be247-115">The checksum passes</span></span>

    <span data-ttu-id="be247-116">Pavyzdžiui, Šis pavyzdys paskatintų DLP kreditinės kortelės numerį ir politikos:</span><span class="sxs-lookup"><span data-stu-id="be247-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="be247-117">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="be247-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="be247-118">Galiojimo laikas: 2/2009</span><span class="sxs-lookup"><span data-stu-id="be247-118">Expires: 2/2009</span></span>

<span data-ttu-id="be247-119">Norėdami gauti daugiau informacijos apie tai, kas reikalinga **Kreditinės kortelės numerį** , galima aptikti jūsų turinį, skaitykite kitame skyriuje šiame straipsnyje: [Kas the jautrios informacijos tipus ieškokite kreditinės kortelės #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="be247-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="be247-120">Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="be247-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  