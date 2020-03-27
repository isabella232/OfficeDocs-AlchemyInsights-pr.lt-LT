---
title: Neveikia JAV banko sąskaitos numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977170"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="2850b-102">DLP problemos su JAV banko sąskaitų numeriais</span><span class="sxs-lookup"><span data-stu-id="2850b-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="2850b-103">**Svarbu:** šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos išliktų labai pasiekiamos – daugiau informacijos rasite ["SharePoint Online" laikinieji funkcijų koregavimai.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="2850b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2850b-104">**DLP problemos su JAV banko sąskaitų numeriais**</span><span class="sxs-lookup"><span data-stu-id="2850b-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="2850b-105">Ar kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **JAV banko sąskaitos numeris,** kai naudojate DLP slaptos informacijos tipą O365?</span><span class="sxs-lookup"><span data-stu-id="2850b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="2850b-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kurios ieškote, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="2850b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="2850b-107">Pvz., **JAV banko sąskaitos numerio** strategija, sukonfigūruota 85 % patikimumo lygiu, įvertinami ir turi būti aptikta, kad taisyklė būtų suaktyvinta:</span><span class="sxs-lookup"><span data-stu-id="2850b-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2850b-108">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 skaitmenų</span><span class="sxs-lookup"><span data-stu-id="2850b-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="2850b-109">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 skaitmenų iš eilės.</span><span class="sxs-lookup"><span data-stu-id="2850b-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="2850b-110">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="2850b-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="2850b-111">**[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP strategija yra 75% įsitikinusi, kad ji aptiko tokio tipo slaptą informaciją, jei 300 simbolių atstumu:</span><span class="sxs-lookup"><span data-stu-id="2850b-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="2850b-112">Paprastoji išraiška Regex_usa_bank_account_number randa šabloną atitinkantį turinį</span><span class="sxs-lookup"><span data-stu-id="2850b-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="2850b-113">Rastas raktinis žodis iš Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="2850b-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="2850b-114">Pvz., jav **banko sąskaitos numerio** strategijos suaktyvinamas šis pavyzdys: tikrinimo sąskaita 78344011</span><span class="sxs-lookup"><span data-stu-id="2850b-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="2850b-115">Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų **aptiktas JAV banko sąskaitos numeris,** ieškokite šiame šio straipsnio skyriuje: [Kokie slaptos informacijos tipai ieško JAV banko sąskaitos numerio](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="2850b-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="2850b-116">Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje</span><span class="sxs-lookup"><span data-stu-id="2850b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  