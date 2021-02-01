---
title: Problemos su autentifikavimo bibliotekomis
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063638"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="e7057-102">Problemos su autentifikavimo bibliotekomis</span><span class="sxs-lookup"><span data-stu-id="e7057-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="e7057-103">["Microsoft" tapatybės platformos autentifikavimo bibliotekose](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) pateikiami "Microsoft" palaikomi ir suderinami kliento ir "tarpinės" bibliotekos.</span><span class="sxs-lookup"><span data-stu-id="e7057-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="e7057-104">"Microsoft" autentifikavimo biblioteka (MSAL) palaiko kelis [autentifikavimo srautus](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) , skirtus naudoti skirtinguose taikomosios programos scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="e7057-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="e7057-105">Norėdami autentifikuoti ir įsigyti atpažinimo ženklus, inicijuokite savo kode naują viešą arba konfidencialią kliento taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="e7057-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="e7057-106">Galite nustatyti kelias konfigūravimo parinktis, kai inicijuojate kliento programą "Microsoft" autentifikavimo bibliotekoje (MSAL).</span><span class="sxs-lookup"><span data-stu-id="e7057-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="e7057-107">Norėdami sužinoti daugiau, peržiūrėkite [taikomosios programos konfigūravimo parinktys](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="e7057-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="e7057-108">**"Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "Azure AD Graph" API (AAD Graph) palaikymo nutraukimas**</span><span class="sxs-lookup"><span data-stu-id="e7057-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="e7057-109">**Nuo birželio 30 d., 2020**, mes nebeįtrauksime jokių naujų "adal" ir "Azure AD Graph" funkcijų.</span><span class="sxs-lookup"><span data-stu-id="e7057-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="e7057-110">Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.</span><span class="sxs-lookup"><span data-stu-id="e7057-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="e7057-111">**Nuo birželio 30 d., 2022**, mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="e7057-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="e7057-112">Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės *gauti jokio techninio palaikymo ar saugos naujinimų*.</span><span class="sxs-lookup"><span data-stu-id="e7057-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="e7057-113">Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.</span><span class="sxs-lookup"><span data-stu-id="e7057-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="e7057-114">**ADAL perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="e7057-114">**ADAL Migration**</span></span>

<span data-ttu-id="e7057-115">Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.</span><span class="sxs-lookup"><span data-stu-id="e7057-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="e7057-116">Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft" proceso metu migruoja jo taikomąsias programas į "MSAL" iki palaikymo termino pabaigos ir užtikrins, kad bus naudingi "MSAL" saugos ir funkcijų patobulinimai.</span><span class="sxs-lookup"><span data-stu-id="e7057-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="e7057-117">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="e7057-117">For more information, see:</span></span>

1. [<span data-ttu-id="e7057-118">Skaityti ADAL DUK</span><span class="sxs-lookup"><span data-stu-id="e7057-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="e7057-119">Sužinokite, kaip perkelti programas pagal platformą</span><span class="sxs-lookup"><span data-stu-id="e7057-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="e7057-120">Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo ISVs arba taikomųjų programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="e7057-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="e7057-121">„Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.</span><span class="sxs-lookup"><span data-stu-id="e7057-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="e7057-122">**„AAD Graph“ perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="e7057-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="e7057-123">Jei naudojate "Azure AD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip [perkelti "AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="e7057-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="e7057-124">Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką.</span><span class="sxs-lookup"><span data-stu-id="e7057-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="e7057-125">Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“.</span><span class="sxs-lookup"><span data-stu-id="e7057-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="e7057-126">Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="e7057-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="e7057-127">"Microsoft" palaikymas taip pat gali suteikti jums sąrašą visų "AAD Graph" naudojimo jūsų nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="e7057-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="e7057-128">Jei norite, kad programa pasiektų duomenis programoje "Microsoft Graph", vartotojas arba administratorius, naudodamas sutikimo procesą, privalo suteikti jam teisingas teises.</span><span class="sxs-lookup"><span data-stu-id="e7057-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="e7057-129">["Microsoft Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference) išvardijamos teisės, susietos su kiekvienu pagrindiniu "Microsoft Graph" API rinkiniu.</span><span class="sxs-lookup"><span data-stu-id="e7057-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="e7057-130">Taip pat pateikiama rekomendacijų, kaip naudoti teises.</span><span class="sxs-lookup"><span data-stu-id="e7057-130">It also provides guidance about how to use the permissions.</span></span>
