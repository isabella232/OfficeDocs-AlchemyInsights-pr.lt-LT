---
title: Neveikia JAV / JUNGTINĖS Karalystės paso numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507306"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="1412e-102">Problemos su DLP - JAV / JK pasų numeriai</span><span class="sxs-lookup"><span data-stu-id="1412e-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="1412e-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="1412e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="1412e-104">**DLP problemos su JAV / JK pasų numeriais**</span><span class="sxs-lookup"><span data-stu-id="1412e-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="1412e-105">Ar turite problemų su **duomenų praradimo prevencija (DLP)** neveikia turinio, kuriame yra **JAV / JK paso numerį,** kai naudojate DLP slaptos informacijos tipą O365?</span><span class="sxs-lookup"><span data-stu-id="1412e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1412e-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kurios ieškote, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="1412e-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="1412e-107">Pvz., **JAV ir Jungtinės Karalystės paso numerio** strategija, sukonfigūruota 75 % patikimumo lygiu, įvertinami toliau nurodyti duomenys, kuriuos reikia aptikti, kad taisyklė būtų suaktyvinta</span><span class="sxs-lookup"><span data-stu-id="1412e-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="1412e-108">**[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devyni skaitmenys</span><span class="sxs-lookup"><span data-stu-id="1412e-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="1412e-109">**[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devyni skaitmenys iš eilės</span><span class="sxs-lookup"><span data-stu-id="1412e-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="1412e-110">**[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="1412e-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="1412e-111">**[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP strategija yra 75% įsitikinusi, kad ji aptiko tokio tipo slaptą informaciją, jei 300 simbolių atstumu:</span><span class="sxs-lookup"><span data-stu-id="1412e-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1412e-112">Funkcija Func_usa_uk_passport randa šabloną atitinkantį turinį.</span><span class="sxs-lookup"><span data-stu-id="1412e-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="1412e-113">Rastas raktinis žodis iš Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="1412e-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="1412e-114">Pvz., šis pavyzdys būtų sukelti **JAV ir Jungtinės Karalystės paso numerio** politika: JAV paso numeris 123456789</span><span class="sxs-lookup"><span data-stu-id="1412e-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="1412e-115">Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų aptiktas JAV/ JUNGTINĖS Karalystės paso numeris, ieškokite šiame šio straipsnio skyriuje: [Kas slaptos informacijos tipai ieško JAV / JUNGTINĖS Karalystės paso numerio](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="1412e-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="1412e-116">Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) šiame straipsnyje</span><span class="sxs-lookup"><span data-stu-id="1412e-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  