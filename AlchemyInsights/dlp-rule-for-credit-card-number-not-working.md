---
title: Neveikia kredito kortelės numerio DLP taisyklė
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679449"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="d84a4-102">DLP problemos su kredito kortelių numeriais</span><span class="sxs-lookup"><span data-stu-id="d84a4-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="d84a4-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d84a4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d84a4-104">**DLP problemos su kredito kortelių numeriais**</span><span class="sxs-lookup"><span data-stu-id="d84a4-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="d84a4-105">Kyla problemų, susijusių su **duomenų praradimo prevencija (DLP)** neveikia turiniui, kuriame yra **kredito kortelės numeris** , kai naudojant DLP slaptą informacijos tipą "O365"?</span><span class="sxs-lookup"><span data-stu-id="d84a4-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d84a4-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija, kad suaktyvintų DLP strategiją, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="d84a4-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="d84a4-107">Pvz., **kredito kortelės strategijos** , sukonfigūruotos naudojant 85% pasikliautinąjį lygį, toliau pateikiami įvertinti ir turi būti aptikti taisyklės, kad būtų galima suaktyvinti:</span><span class="sxs-lookup"><span data-stu-id="d84a4-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d84a4-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 skaitmenų, kuriuos galima formatuoti arba nesuformatuoti (dddddddddddddddd) ir turi praeiti Luhn testą.</span><span class="sxs-lookup"><span data-stu-id="d84a4-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="d84a4-109">**[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Labai sudėtingas ir tvirtas raštas, kuris aptinka korteles iš visų didžiųjų prekinių ženklų visame pasaulyje, įskaitant visa, MasterCard, Discover Card, JCB, American Express, dovanų korteles ir Diner korteles.</span><span class="sxs-lookup"><span data-stu-id="d84a4-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="d84a4-110">**[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Taip, Luhn kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="d84a4-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="d84a4-111">**[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP strategija yra 85% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:</span><span class="sxs-lookup"><span data-stu-id="d84a4-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d84a4-112">Funkcija Func_credit_card randa turinį, atitinkantį raštą.</span><span class="sxs-lookup"><span data-stu-id="d84a4-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d84a4-113">Patenkinama viena iš šių veiksmų:</span><span class="sxs-lookup"><span data-stu-id="d84a4-113">One of the following is true:</span></span>

  - <span data-ttu-id="d84a4-114">Randamas raktažodis iš Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="d84a4-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="d84a4-115">Randamas raktažodis iš Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="d84a4-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="d84a4-116">Funkcija Func_expiration_date randa datą reikiamu datos formatu.</span><span class="sxs-lookup"><span data-stu-id="d84a4-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="d84a4-117">Kontrolinė suma eina</span><span class="sxs-lookup"><span data-stu-id="d84a4-117">The checksum passes</span></span>

    <span data-ttu-id="d84a4-118">Pvz., Šis pavyzdys turėtų suaktyvinti DLP kredito kortelės numerio strategiją:</span><span class="sxs-lookup"><span data-stu-id="d84a4-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="d84a4-119">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="d84a4-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="d84a4-120">Galiojimo laikas: 2/2009</span><span class="sxs-lookup"><span data-stu-id="d84a4-120">Expires: 2/2009</span></span>

<span data-ttu-id="d84a4-121">Daugiau informacijos apie tai, ko reikia **kredito kortelės numeriui** aptikti jūsų turinyje, ieškokite šiame straipsnyje šiame straipsnyje: [kas yra slaptos informacijos tipai ieškoti kredito kortelės #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="d84a4-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="d84a4-122">Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d84a4-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  