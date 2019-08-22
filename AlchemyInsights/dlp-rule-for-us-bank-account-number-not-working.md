---
title: DLP taisyklė mūsų banko sąskaitos numeris ne darbo
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
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529883"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="61c86-102">DLP problemų su mūsų banko sąskaitų numeriai</span><span class="sxs-lookup"><span data-stu-id="61c86-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="61c86-103">Ar iškilo problemų su **Duomenų praradimo prevencijos (DLP)** ne darbo turinio su **JAV banko sąskaitos numerį** , naudojant DLP slaptos informacijos tipo O365?</span><span class="sxs-lookup"><span data-stu-id="61c86-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="61c86-104">Jei taip, įsitikinkite, kad jūsų turinys yra reikalingą informaciją, DLP strategijos ieško kai ji įvertinta.</span><span class="sxs-lookup"><span data-stu-id="61c86-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="61c86-105">Pavyzdžiui, **JAV banko sąskaitos numeris** politikos suderintas su 85 % pasikliovimo lygmeniu, toliau yra vertinami ir turi būti nustatytas būtų sukelti taisyklė:</span><span class="sxs-lookup"><span data-stu-id="61c86-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="61c86-106">**[Formatu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 skaitmenų</span><span class="sxs-lookup"><span data-stu-id="61c86-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="61c86-107">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 nuosekli skaitmenų seka.</span><span class="sxs-lookup"><span data-stu-id="61c86-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="61c86-108">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra jokių kontrolinė suma</span><span class="sxs-lookup"><span data-stu-id="61c86-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="61c86-109">**[Raiškos:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika yra 75 % tikimybė, kad jis aptiko tokia slaptos informacijos jei per arti 300 simbolių:</span><span class="sxs-lookup"><span data-stu-id="61c86-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="61c86-110">Reguliarios išraiškos Regex_usa_bank_account_number randa modelis atitinkantis turinys</span><span class="sxs-lookup"><span data-stu-id="61c86-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="61c86-111">Raktinis žodis Keyword_usa_Bank_Account yra nustatyta.</span><span class="sxs-lookup"><span data-stu-id="61c86-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="61c86-112">Pavyzdžiui, Šis pavyzdys paskatintų politikos **JAV banko sąskaitos numeris** : Atsiskaitomoji sąskaita 78344011</span><span class="sxs-lookup"><span data-stu-id="61c86-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="61c86-113">Norėdami gauti daugiau informacijos apie tai, kas reikalinga **JAV banko sąskaitos numerį** , galima aptikti jūsų turinį, skaitykite kitame skyriuje šiame straipsnyje: [Kas the jautrios informacijos tipus ieškokite JAV banko sąskaitos numeris](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="61c86-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="61c86-114">Naudojant įvairių įmontuota slapta informacija tipo, skaitykite šį straipsnį informacijos apie tai, kas yra reikalingi kitokie: [kas the jautrios informacijos tipus ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="61c86-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  