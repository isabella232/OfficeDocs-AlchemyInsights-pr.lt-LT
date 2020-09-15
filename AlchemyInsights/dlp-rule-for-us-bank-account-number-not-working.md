---
title: "\"DLP\" taisyklės, skirtos JAV banko sąskaitos numeriui"
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679304"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="e3cce-102">"DLP" problemos su JAV banko sąskaitų numeriais</span><span class="sxs-lookup"><span data-stu-id="e3cce-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="e3cce-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e3cce-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e3cce-104">**"DLP" problemos su JAV banko sąskaitų numeriais**</span><span class="sxs-lookup"><span data-stu-id="e3cce-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="e3cce-105">Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **JAV banko sąskaitos numeris** , kai naudojant DLP slaptą informacijos tipą "O365"?</span><span class="sxs-lookup"><span data-stu-id="e3cce-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="e3cce-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, kas yra DLP strategija, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="e3cce-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="e3cce-107">Pvz., **JAV banko sąskaitos numerio** strategija, sukonfigūruota su 85% pasikliovimo lygiu, yra vertinama ir turi būti nustatyta taisyklės, kad suaktyvintų:</span><span class="sxs-lookup"><span data-stu-id="e3cce-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="e3cce-108">**[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 skaitmenys</span><span class="sxs-lookup"><span data-stu-id="e3cce-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="e3cce-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 iš eilės skaitmenys.</span><span class="sxs-lookup"><span data-stu-id="e3cce-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="e3cce-110">**[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra jokios kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="e3cce-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="e3cce-111">**[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP strategija yra 75% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:</span><span class="sxs-lookup"><span data-stu-id="e3cce-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="e3cce-112">Įprastas reiškinys Regex_usa_bank_account_number randa turinį, atitinkantį raštą</span><span class="sxs-lookup"><span data-stu-id="e3cce-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="e3cce-113">Randamas raktažodis iš Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="e3cce-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="e3cce-114">Pvz., Šis pavyzdys sukeltų **JAV banko sąskaitos numerio** strategiją: paskyros 78344011</span><span class="sxs-lookup"><span data-stu-id="e3cce-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="e3cce-115">Daugiau informacijos apie tai, ko reikia **JAV banko sąskaitos numeriui** aptikti jūsų turinyje, ieškokite šiame straipsnyje šiame straipsnyje: [kokie jautrūs informacijos tipai tinka JAV banko sąskaitos numeriui](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="e3cce-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="e3cce-116">Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e3cce-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  