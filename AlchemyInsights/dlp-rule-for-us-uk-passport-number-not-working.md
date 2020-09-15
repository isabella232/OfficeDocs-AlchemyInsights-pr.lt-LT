---
title: "\"DLP\" taisyklė, skirta JAV/JK paso numeris neveikia"
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679232"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="0cdb8-102">Problemos su DLP-US/UK paso numeriais</span><span class="sxs-lookup"><span data-stu-id="0cdb8-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="0cdb8-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0cdb8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0cdb8-104">**"DLP" problemos su JAV/JK pasų numeriai**</span><span class="sxs-lookup"><span data-stu-id="0cdb8-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="0cdb8-105">Kyla problemų dėl **duomenų praradimo prevencijos (DLP)** neveikia turinio, kuriame yra **JAV/JK paso numeris** , kai naudojant DLP slaptą informacijos tipą "O365"?</span><span class="sxs-lookup"><span data-stu-id="0cdb8-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0cdb8-106">Jei taip, įsitikinkite, kad jūsų turinyje yra reikalinga informacija apie tai, kas yra DLP strategija, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="0cdb8-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0cdb8-107">Pvz., **JAV/JK paso numerio** strategiją, sukonfigūruotą su 75% pasikliovimo lygiu, toliau pateikta informacija vertinama ir turi būti nustatyta taisyklės, kad suaktyvintų</span><span class="sxs-lookup"><span data-stu-id="0cdb8-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="0cdb8-108">**[Formatas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devyni skaitmenys</span><span class="sxs-lookup"><span data-stu-id="0cdb8-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="0cdb8-109">**[Raštas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devyni iš eilės skaitmenys</span><span class="sxs-lookup"><span data-stu-id="0cdb8-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="0cdb8-110">**[Kontrolinė suma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, nėra jokios kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="0cdb8-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0cdb8-111">**[Apibrėžimas:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP strategija yra 75% įsitikinę, kad jis aptinka šio tipo slaptą informaciją, jei "300" simbolių arti:</span><span class="sxs-lookup"><span data-stu-id="0cdb8-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0cdb8-112">Funkcija Func_usa_uk_passport randa turinį, atitinkantį raštą.</span><span class="sxs-lookup"><span data-stu-id="0cdb8-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0cdb8-113">Randamas raktažodis iš Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="0cdb8-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="0cdb8-114">Pavyzdžiui, Šis pavyzdys sukeltų **JAV/JK paso numerio** strategiją: JAV paso numeris 123456789</span><span class="sxs-lookup"><span data-stu-id="0cdb8-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="0cdb8-115">Daugiau informacijos apie tai, ko reikia, kad būtų aptiktas jūsų turinio JAV/JK paso numeris, ieškokite šiame straipsnyje šiame straipsnyje: [kokie jautrūs informacijos tipai tinka JAV/JK paso numeriui](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="0cdb8-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="0cdb8-116">Naudodami kitą įtaisytąjį slaptą informacijos tipą, skaitykite šį straipsnį informacijos apie tai, ko reikia kitiems tipams: [kaip atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0cdb8-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  