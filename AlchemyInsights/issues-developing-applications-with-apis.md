---
title: Problemos kuriant taikomąsias programas su API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974623"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="a790c-102">Problemos kuriant taikomąsias programas su API</span><span class="sxs-lookup"><span data-stu-id="a790c-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="a790c-103">Norėdami pradėti naudoti "Azure Active Directory Graph" API, peržiūrėkite " [AZURE ad GRAPH API" greitojo pasirengimo darbui vadovą](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) arba peržiūrėkite [INTERAKTYVIĄ "Azure AD Graph" API nuorodų dokumentaciją](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="a790c-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="a790c-104">**"Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "Azure AD Graph" API (AAD Graph) palaikymo nutraukimas**</span><span class="sxs-lookup"><span data-stu-id="a790c-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="a790c-105">**Nuo birželio 30 d., 2020**, mes nebeįtrauksime jokių naujų "adal" ir "Azure AD Graph" funkcijų.</span><span class="sxs-lookup"><span data-stu-id="a790c-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="a790c-106">Mes ir toliau suteiksime techninio palaikymo ir saugos naujinimus, tačiau nebepateiksime funkcijų naujinimų.</span><span class="sxs-lookup"><span data-stu-id="a790c-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="a790c-107">**Nuo birželio 30 d., 2022**, mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="a790c-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="a790c-108">Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės gauti jokio techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="a790c-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="a790c-109">Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.</span><span class="sxs-lookup"><span data-stu-id="a790c-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="a790c-110">**ADAL perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="a790c-110">**ADAL Migration**</span></span>

<span data-ttu-id="a790c-111">Rekomenduojame naujinti į ["Microsoft" autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kuri turi naujausias funkcijas ir saugos naujinimus.</span><span class="sxs-lookup"><span data-stu-id="a790c-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="a790c-112">Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft" proceso metu migruoja jo taikomąsias programas į "MSAL" iki palaikymo termino pabaigos ir užtikrins, kad jos bus naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.</span><span class="sxs-lookup"><span data-stu-id="a790c-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="a790c-113">[Perskaitykite ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="a790c-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="a790c-114">[Sužinokite, kaip perkelti taikomąsias programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="a790c-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="a790c-115">Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo ISVs arba taikomųjų programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="a790c-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a790c-116">"Microsoft" palaikymas taip pat gali suteikti jums visų ne "Microsoft" ADAL taikomųjų programų sąrašą savo nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="a790c-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="a790c-117">**AAD Graph perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="a790c-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="a790c-118">Jei naudojate "Azure AD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip perkelti ["AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="a790c-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="a790c-119">[Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="a790c-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="a790c-120">"Azure App" registracijos portale rodoma, kurios taikomosios programos naudoja AAD grafiką.</span><span class="sxs-lookup"><span data-stu-id="a790c-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="a790c-121">Rekomenduojame Peržiūrėti visus savo taikomųjų programų šaltinio kodus ir, jei reikia, pasiekti bet kokius ISVs arba taikomųjų programų teikėjus.</span><span class="sxs-lookup"><span data-stu-id="a790c-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a790c-122">"Microsoft" palaikymas taip pat gali suteikti jums sąrašą visų "AAD Graph" naudojimo jūsų nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="a790c-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="a790c-123">Jei norite, kad programa pasiektų duomenis programoje "Microsoft Graph", vartotojas arba administratorius, naudodamas sutikimo procesą, privalo suteikti jam teisingas teises.</span><span class="sxs-lookup"><span data-stu-id="a790c-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="a790c-124">["Microsoft Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) išvardijamos teisės, susietos su kiekvienu pagrindiniu "Microsoft Graph" API rinkiniu.</span><span class="sxs-lookup"><span data-stu-id="a790c-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="a790c-125">Taip pat pateikiama rekomendacijų, kaip naudoti teises.</span><span class="sxs-lookup"><span data-stu-id="a790c-125">It also provides guidance about how to use the permissions.</span></span>
