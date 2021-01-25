---
title: Problemos kuriant taikomąsias programas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974470"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="450fe-102">Problemos kuriant taikomąsias programas</span><span class="sxs-lookup"><span data-stu-id="450fe-102">Issues developing applications</span></span>

<span data-ttu-id="450fe-103">Norėdami pašalinti Dažniausias "Azure Active Directory" (AD) programų kūrimo problemas, skaitykite šiuos straipsnius:</span><span class="sxs-lookup"><span data-stu-id="450fe-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="450fe-104">Matau problemų prisijungiant prie taikomosios programos (-ų) naudojant tik "Chrome" naršyklę</span><span class="sxs-lookup"><span data-stu-id="450fe-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="450fe-105">Nežinau, kaip pakeisti atpažinimo ženklo naudojimo numatytuosius parametrus mano taikomojoje programoje</span><span class="sxs-lookup"><span data-stu-id="450fe-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="450fe-106">Aš painiojama apie tai, kaip veikia taikomųjų programų sutikimas</span><span class="sxs-lookup"><span data-stu-id="450fe-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="450fe-107">Nežinau, kaip suteikti teises savo taikomajai programai</span><span class="sxs-lookup"><span data-stu-id="450fe-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="450fe-108">Nesuprantu skirtumo tarp įgaliotųjų ir taikomosios programos teisių</span><span class="sxs-lookup"><span data-stu-id="450fe-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="450fe-109">\*" **Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "AZURE ad Graph" API (AAD grafikas) palaikymo pabaiga**</span><span class="sxs-lookup"><span data-stu-id="450fe-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="450fe-110">Nuo birželio 30 d., 2020, nebegalėsime įtraukti jokių naujų funkcijų į "Azure Active Directory" autentifikavimo biblioteką (ADAL) ir "Azure AD Graph API" (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="450fe-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="450fe-111">Mes ir toliau suteiksime techninio palaikymo ir saugos naujinimus, tačiau nebepateiksime funkcijų naujinimų.</span><span class="sxs-lookup"><span data-stu-id="450fe-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="450fe-112">Nuo birželio 30 d., 2022, mes užbaigsime ADAL ir AAD Graph palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="450fe-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="450fe-113">Dėl šios sąlygos, toliau pateikiami padariniai:</span><span class="sxs-lookup"><span data-stu-id="450fe-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="450fe-114">Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės gauti jokio techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="450fe-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="450fe-115">Taikomosios programos, naudojančios AAD grafiką po šio laiko, gali nebegauti atsakymų iš AAD diagramos galinio punkto</span><span class="sxs-lookup"><span data-stu-id="450fe-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="450fe-116">−*Adal perkėlimas*\*</span><span class="sxs-lookup"><span data-stu-id="450fe-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="450fe-117">Jei naudojate "Microsoft" taikomąsias programas, rekomenduojame naujinti į "Microsoft" autentifikavimo biblioteką (MSAL), kuri turi naujausias funkcijas ir saugos naujinimus.</span><span class="sxs-lookup"><span data-stu-id="450fe-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="450fe-118">Ši rekomendacija parengta atsižvelgiant į tai, kad "Microsoft" pradeda perkelti savo taikomąsias programas į MSAL iki palaikymo termino pabaigos.</span><span class="sxs-lookup"><span data-stu-id="450fe-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="450fe-119">"Microsoft" vykdomas "Microsoft" perkėlimas į "MSAL" užtikrina, kad taikomosios programos naudos iš MSAL vykstančių saugos ir funkcijų patobulinimų.</span><span class="sxs-lookup"><span data-stu-id="450fe-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="450fe-120">DUK apie ADAL</span><span class="sxs-lookup"><span data-stu-id="450fe-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="450fe-121">Sužinokite, kaip perkelti taikomąsias programas pagal platformą</span><span class="sxs-lookup"><span data-stu-id="450fe-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="450fe-122">Jei jums reikia pagalbos suprasti, kurią iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su bet kuriuo nepriklausomu programinės įrangos pardavėjais (ISVs) arba taikomųjų programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="450fe-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="450fe-123">"Microsoft" palaikymas taip pat gali suteikti jums visų ne "Microsoft" ADAL taikomųjų programų sąrašą savo nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="450fe-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="450fe-124">**AAD Graph perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="450fe-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="450fe-125">Jei naudojate "AAD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip perkelti "AAD Graph" taikomąsias programas į "Microsoft Graph":</span><span class="sxs-lookup"><span data-stu-id="450fe-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="450fe-126">[Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="450fe-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="450fe-127">"Azure App" registracijos portale rodoma, kurios taikomosios programos naudoja AAD grafiką.</span><span class="sxs-lookup"><span data-stu-id="450fe-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="450fe-128">Rekomenduojame Peržiūrėti visus savo taikomųjų programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriais nepriklausomais programinės įrangos tiekėjais (ISVs) arba taikomųjų programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="450fe-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="450fe-129">"Microsoft" palaikymas taip pat gali suteikti informacijos apie "AAD Graph" naudojimą jūsų nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="450fe-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







