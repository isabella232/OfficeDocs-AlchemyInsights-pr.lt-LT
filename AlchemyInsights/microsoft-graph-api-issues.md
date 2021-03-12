---
title: "\"Microsoft Graph\" API problemos"
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714153"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="8c650-102">"Microsoft Graph" API problemos</span><span class="sxs-lookup"><span data-stu-id="8c650-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="8c650-103">Ši tema taip pat gali būti taikoma kūrėjams, kurie vis dar naudoja "Azure AD Graph API".</span><span class="sxs-lookup"><span data-stu-id="8c650-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="8c650-104">Tačiau **primygtinai** rekomenduojama naudoti "Microsoft Graph" visiems jūsų katalogo, tapatybės ir "Access" valdymo scenarijams.</span><span class="sxs-lookup"><span data-stu-id="8c650-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="8c650-105">**Autentifikavimo arba autorizavimo problemos**</span><span class="sxs-lookup"><span data-stu-id="8c650-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="8c650-106">Jei jūsų programai **nepavyksta įsigyti žetonų** norint paskambinti "Microsoft Graph", pasirinkite problemą, kad gautumėte " **Access" atpažinimo ženklo (autentifikavimo)** "Microsoft Graph" kategoriją, kad gautumėte daugiau konkrečios žinyno ir palaikymo šioje temoje.</span><span class="sxs-lookup"><span data-stu-id="8c650-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="8c650-107">Jei jūsų programa **gauna "401" arba "403" autorizavimo klaidas** , kai skambinate "Microsoft Graph", pasirinkite "Microsoft Graph API" kategoriją gauti prieigą prie " **Access Denied" (leidimas)** , kad šioje temoje gautumėte konkretesnį žinyną ir palaikymą.</span><span class="sxs-lookup"><span data-stu-id="8c650-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="8c650-108">**Noriu naudoti "Microsoft Graph", bet nežinote, nuo ko pradėti**</span><span class="sxs-lookup"><span data-stu-id="8c650-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="8c650-109">"Microsoft Graph" apžvalga</span><span class="sxs-lookup"><span data-stu-id="8c650-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="8c650-110">Tapatybės ir "Access" valdymo apžvalga programoje "Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="8c650-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="8c650-111">Darbo pradžia "Microsoft Graph" taikomųjų programų kūrimas</span><span class="sxs-lookup"><span data-stu-id="8c650-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="8c650-112">**"Microsoft Graph Explorer"** – jūsų nuomotojo arba demonstracinio kompiuterio "Microsoft Graph" API bandymas</span><span class="sxs-lookup"><span data-stu-id="8c650-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="8c650-113">**Noriu naudoti "Microsoft Graph", tačiau ar ji palaiko "v 1.0" katalogo API, kurių man reikia?**</span><span class="sxs-lookup"><span data-stu-id="8c650-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="8c650-114">"Microsoft Graph" yra rekomenduojamas katalogo, tapatybės ir "Access" valdymo API.</span><span class="sxs-lookup"><span data-stu-id="8c650-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="8c650-115">Tačiau vis dar yra kelios spragos tarp to, kas įmanoma, "Azure AD Graph" ir "Microsoft Graph".</span><span class="sxs-lookup"><span data-stu-id="8c650-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="8c650-116">Peržiūrėkite šiuos straipsnius, kuriuose Akcentuokite naujausius skirtumus, kurie padės jums pasirinkti:</span><span class="sxs-lookup"><span data-stu-id="8c650-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="8c650-117">Išteklių tipo skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="8c650-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="8c650-118">Ypatybių skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="8c650-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="8c650-119">"Azure AD" ir "Microsoft Graph" metodo skirtumai</span><span class="sxs-lookup"><span data-stu-id="8c650-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="8c650-120">**Mano skambinimo API neveikia – kur galiu atlikti daugiau bandymų?**</span><span class="sxs-lookup"><span data-stu-id="8c650-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="8c650-121">**"Microsoft Graph Explorer"** – Išbandykite "Microsoft Graph" API savo nuomotojuje arba "demo" nuomotojuje, taip pat peržiūrėkite **užklausų užklausas** programoje "Microsoft Graph Explorer".</span><span class="sxs-lookup"><span data-stu-id="8c650-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="8c650-122">**Mano programa yra per lėta ir taip pat yra Throttled. Kokius patobulinimus galiu padaryti?**</span><span class="sxs-lookup"><span data-stu-id="8c650-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="8c650-123">Atsižvelgiant į jūsų scenarijų, jūsų dispozicijoje yra įvairių parinkčių, kad jūsų programa būtų efektyvesnė, o kai kuriais atvejais, mažiau linkę ją naudoti (kai skambinate per daug kartų).</span><span class="sxs-lookup"><span data-stu-id="8c650-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="8c650-124">"Microsoft Graph" geriausios praktikos</span><span class="sxs-lookup"><span data-stu-id="8c650-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="8c650-125">Užklausų grupavimas</span><span class="sxs-lookup"><span data-stu-id="8c650-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="8c650-126">Keitimų sekimas naudojant Delta užklausą</span><span class="sxs-lookup"><span data-stu-id="8c650-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="8c650-127">Gaukite pranešimus apie keitimą naudodami webkablius</span><span class="sxs-lookup"><span data-stu-id="8c650-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="8c650-128">Ribojimo gairės</span><span class="sxs-lookup"><span data-stu-id="8c650-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="8c650-129">**Kur galiu gauti daugiau informacijos apie klaidas ir žinomas problemas?**</span><span class="sxs-lookup"><span data-stu-id="8c650-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="8c650-130">"Microsoft Graph" klaidos atsakymo informacija</span><span class="sxs-lookup"><span data-stu-id="8c650-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="8c650-131">Žinomos "Microsoft Graph" problemos</span><span class="sxs-lookup"><span data-stu-id="8c650-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="8c650-132">**Kur galiu patikrinti paslaugų pasiekiamumo ir ryšio būseną?**</span><span class="sxs-lookup"><span data-stu-id="8c650-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="8c650-133">Tarnybų pasiekiamumo ir ryšio su pagrindinėmis tarnybomis, kurias galima pasiekti naudojant "Microsoft Graph", paslaugos gali turėti įtakos bendram "Microsoft Graph" pasiekiamumui ir veikimui.</span><span class="sxs-lookup"><span data-stu-id="8c650-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="8c650-134">"Azure Active Directory" tarnybos sveikatai patikrinkite **saugos + tapatybės** tarnybų būseną, išvardytas "Azure" [būsenos puslapyje](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="8c650-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="8c650-135">"Office" tarnyboms, kurios prisideda prie "Microsoft Graph", patikrinkite tarnybų, išvardintų " [Office" tarnybos sveikatos ataskaitų](https://portal.office.com/adminportal/home#/servicehealth)srityje, būseną.</span><span class="sxs-lookup"><span data-stu-id="8c650-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8c650-136">"Microsoft Graph" autorizavimo klaidos gali kilti dėl kelių skirtingų problemų, kurių dauguma generuoja "401" arba "403" klaidą.</span><span class="sxs-lookup"><span data-stu-id="8c650-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="8c650-137">Pavyzdžiui, toliau nurodyti būdai gali sukelti autorizavimo klaidas:</span><span class="sxs-lookup"><span data-stu-id="8c650-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="8c650-138">Netinkami [atpažinimo ženklo gavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="8c650-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="8c650-139">Prastai konfigūruotos [teisių aprėptys](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="8c650-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="8c650-140">[Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkumas</span><span class="sxs-lookup"><span data-stu-id="8c650-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="8c650-141">\**_„Azure Active Directory“ autentifikavimo bibliotekos (ADAL) ir „Azure AD Graph“ API („AAD Graph“) palaikymo pabaiga_* _</span><span class="sxs-lookup"><span data-stu-id="8c650-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="8c650-142">\* Nuo birželio 30 d., 2020 \* \*, mes nebeįtrauksime jokių naujų funkcijų į ADAL ir Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="8c650-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="8c650-143">Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.</span><span class="sxs-lookup"><span data-stu-id="8c650-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="8c650-144">**Nuo birželio 30 d., 2022**, mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.</span><span class="sxs-lookup"><span data-stu-id="8c650-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="8c650-145">Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės *gauti jokio techninio palaikymo ar saugos naujinimų*.</span><span class="sxs-lookup"><span data-stu-id="8c650-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="8c650-146">Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.</span><span class="sxs-lookup"><span data-stu-id="8c650-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="8c650-147">**ADAL perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="8c650-147">**ADAL Migration**</span></span>

<span data-ttu-id="8c650-148">Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.</span><span class="sxs-lookup"><span data-stu-id="8c650-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="8c650-149">Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft" proceso metu migruoja jo taikomąsias programas į "MSAL" iki palaikymo termino pabaigos ir užtikrins, kad jos bus naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.</span><span class="sxs-lookup"><span data-stu-id="8c650-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="8c650-150">Skaityti ADAL DUK</span><span class="sxs-lookup"><span data-stu-id="8c650-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="8c650-151">Sužinokite, kaip perkelti programas pagal platformą</span><span class="sxs-lookup"><span data-stu-id="8c650-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="8c650-152">Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo ISVs arba taikomųjų programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="8c650-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8c650-153">„Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.</span><span class="sxs-lookup"><span data-stu-id="8c650-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8c650-154">**„AAD Graph“ perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="8c650-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="8c650-155">Jei naudojate "Azure AD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip [perkelti "AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="8c650-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="8c650-156">[Mūsų perkėlimo kontroliniame sąraše apibūdinama darbo pradžia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="8c650-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="8c650-157">Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“.</span><span class="sxs-lookup"><span data-stu-id="8c650-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8c650-158">Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais.</span><span class="sxs-lookup"><span data-stu-id="8c650-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8c650-159">"Microsoft" palaikymas taip pat gali suteikti jums sąrašą visų "AAD Graph" naudojimo jūsų nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="8c650-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="8c650-160">Jei norite, kad programa pasiektų duomenis programoje "Microsoft Graph", vartotojas arba administratorius, naudodamas sutikimo procesą, privalo suteikti jam teisingas teises.</span><span class="sxs-lookup"><span data-stu-id="8c650-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="8c650-161">["Microsoft Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference) išvardijamos teisės, susietos su kiekvienu pagrindiniu "Microsoft Graph" API rinkiniu.</span><span class="sxs-lookup"><span data-stu-id="8c650-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="8c650-162">Taip pat pateikiama rekomendacijų, kaip naudoti teises.</span><span class="sxs-lookup"><span data-stu-id="8c650-162">It also provides guidance about how to use the permissions.</span></span>
