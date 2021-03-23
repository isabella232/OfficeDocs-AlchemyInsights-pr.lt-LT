---
title: Darbas su autentifikavimo bibliotekomis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035827"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="4da6e-102">Darbas su autentifikavimo bibliotekomis</span><span class="sxs-lookup"><span data-stu-id="4da6e-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="4da6e-103">Norėdami išspręsti "Microsoft" autentifikavimo bibliotekos (MSAL) problemą, atlikite šiuos rekomenduojamus veiksmus:</span><span class="sxs-lookup"><span data-stu-id="4da6e-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="4da6e-104">**Darbas su MSAL**: ["Microsoft" tapatybės platformos autentifikavimo bibliotekos](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – šiame straipsnyje rodomas kelių taikomųjų programų tipų "Microsoft" autentifikavimo bibliotekos palaikymas.</span><span class="sxs-lookup"><span data-stu-id="4da6e-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="4da6e-105">Jis turi saitų su bibliotekos šaltinio kodu; kur gauti paketo programos projektui; ir ar biblioteka palaiko vartotojo prisijungimą (autentifikavimas), prieigą prie apsaugotų žiniatinklio API (autorizavimą) arba abu.</span><span class="sxs-lookup"><span data-stu-id="4da6e-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="4da6e-106">**Autentifikavimo trikčių šalinimas**: msal palaiko kelis autentifikavimo srautus, skirtus naudoti skirtinguose taikomosios programos scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="4da6e-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="4da6e-107">Atsižvelgiant į tai, kaip jūsų kliento programa yra sukurta, MSAL gali naudoti vieną ar daugiau autentifikavimo srautų, kuriuos palaiko "Microsoft" tapatybės platforma.</span><span class="sxs-lookup"><span data-stu-id="4da6e-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="4da6e-108">Šie srautai gali pateikti kelių tipų atpažinimo ženklus ir autorizavimo kodus ir reikalauti skirtingų žetonų, kad jie galėtų dirbti.</span><span class="sxs-lookup"><span data-stu-id="4da6e-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="4da6e-109">" **Access" žetonai**: ["Microsoft" tapatybės platformos prieigos žetonai](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Sužinokite, kaip jūsų API gali patvirtinti ir naudoti "Access" atpažinimo ženklo teiginius.</span><span class="sxs-lookup"><span data-stu-id="4da6e-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="4da6e-110">Visi šiame straipsnyje nurodyti dokumentai, išskyrus tuos atvejus, kai pažymėta, taikomi tik žetonams, kurie buvo išduoti jūsų įregistruotam API.</span><span class="sxs-lookup"><span data-stu-id="4da6e-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="4da6e-111">Jis netaikomas žetonams, išduodamais "Microsoft" valdomoms API, taip pat šie žetonai negali būti naudojami norint patikrinti, kaip "Microsoft" tapatybės platforma pateiks Jūsų kuriamos API atpažinimo ženklus.</span><span class="sxs-lookup"><span data-stu-id="4da6e-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="4da6e-112">**"Azure Active Directory" autentifikavimo bibliotekos (ADAL) palaikymo pabaiga**</span><span class="sxs-lookup"><span data-stu-id="4da6e-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="4da6e-113">**Nuo birželio 30 d., 2020,** mes nebeįtrauksime jokių naujų "adal" ir "Azure AD Graph" funkcijų.</span><span class="sxs-lookup"><span data-stu-id="4da6e-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="4da6e-114">Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.</span><span class="sxs-lookup"><span data-stu-id="4da6e-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="4da6e-115">**Nuo birželio 30 d., 2022,** mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="4da6e-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="4da6e-116">Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės *gauti jokio techninio palaikymo ar saugos naujinimų*.</span><span class="sxs-lookup"><span data-stu-id="4da6e-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="4da6e-117">Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.</span><span class="sxs-lookup"><span data-stu-id="4da6e-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="4da6e-118">**ADAL perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="4da6e-118">**ADAL Migration**</span></span>

- <span data-ttu-id="4da6e-119">Rekomenduojame naujinti į MSAL, kuriame yra naujausios funkcijos ir saugos naujinimai.</span><span class="sxs-lookup"><span data-stu-id="4da6e-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="4da6e-120">Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft", siekdama perkelti savo taikomąsias programas į MSAL iki palaikymo termino pabaigos, užtikrins, kad jos bus naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.</span><span class="sxs-lookup"><span data-stu-id="4da6e-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="4da6e-121">[Perskaitykite ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="4da6e-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="4da6e-122">[Sužinokite, kaip perkelti taikomąsias programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="4da6e-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="4da6e-123">Jei perskaitę programos platformos vadovą turite papildomų klausimų, galite skelbti " [Microsoft" Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) su žymomis [Azure – AD-adal – nuteistųjų] arba atidaryti problemą bibliotekoje "GitHub" saugykloje.</span><span class="sxs-lookup"><span data-stu-id="4da6e-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="4da6e-124">Peržiūrėkite " **Msal" apžvalgos** straipsnio skyrių [kalbos ir sistemos](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) , kad būtų galima susieti su kiekviena biblioteka atpirkimo.</span><span class="sxs-lookup"><span data-stu-id="4da6e-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="4da6e-125">**Jei reikia pagalbos norint suprasti, kurios programos naudoja ADAL**, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus.</span><span class="sxs-lookup"><span data-stu-id="4da6e-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="4da6e-126">Jei reikia, susisiekite su visais nepriklausomais programinės įrangos tiekėjais (ISVs) arba taikomųjų programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="4da6e-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="4da6e-127">„Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.</span><span class="sxs-lookup"><span data-stu-id="4da6e-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







