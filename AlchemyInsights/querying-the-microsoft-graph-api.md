---
title: "\"Microsoft Graph\" API užklausų užklausa"
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974423"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="2f397-102">"Microsoft Graph" API užklausų užklausa</span><span class="sxs-lookup"><span data-stu-id="2f397-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="2f397-103">Ši tema taip pat gali būti taikoma kūrėjams, kurie vis dar naudoja "Azure AD Graph API".</span><span class="sxs-lookup"><span data-stu-id="2f397-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="2f397-104">Tačiau **primygtinai** rekomenduojama naudoti "Microsoft Graph" visiems jūsų katalogo, tapatybės ir "Access" valdymo scenarijams.</span><span class="sxs-lookup"><span data-stu-id="2f397-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="2f397-105">**Autentifikavimo arba autorizavimo problemos**</span><span class="sxs-lookup"><span data-stu-id="2f397-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="2f397-106">Jei jūsų programai **nepavyksta įsigyti žetonų** norint paskambinti "Microsoft Graph", pasirinkite problemą, kad gautumėte " **Access" atpažinimo ženklo (autentifikavimo)** "Microsoft Graph" kategoriją, kad gautumėte daugiau konkrečios žinyno ir palaikymo šioje temoje.</span><span class="sxs-lookup"><span data-stu-id="2f397-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="2f397-107">Jei jūsų programa **gauna "401" arba "403" autorizavimo klaidas** , kai skambinate "Microsoft Graph", pasirinkite "Microsoft Graph API" kategoriją gauti prieigą prie " **Access Denied" (leidimas)** , kad šioje temoje gautumėte konkretesnį žinyną ir palaikymą.</span><span class="sxs-lookup"><span data-stu-id="2f397-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="2f397-108">**Noriu naudoti "Microsoft Graph", bet nežinote, nuo ko pradėti**</span><span class="sxs-lookup"><span data-stu-id="2f397-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="2f397-109">Norėdami sužinoti daugiau apie "Microsoft Graph", žiūrėkite:</span><span class="sxs-lookup"><span data-stu-id="2f397-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="2f397-110">"Microsoft Graph" apžvalga</span><span class="sxs-lookup"><span data-stu-id="2f397-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="2f397-111">Tapatybės ir "Access" valdymo apžvalga programoje "Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="2f397-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="2f397-112">Darbo pradžia "Microsoft Graph" taikomųjų programų kūrimas</span><span class="sxs-lookup"><span data-stu-id="2f397-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="2f397-113">**"Microsoft Graph Explorer"** – jūsų nuomotojo arba demonstracinio kompiuterio "Microsoft Graph" API bandymas</span><span class="sxs-lookup"><span data-stu-id="2f397-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="2f397-114">**Noriu naudoti "Microsoft Graph", tačiau ar ji palaiko "v 1.0" katalogo API, kurių man reikia?**</span><span class="sxs-lookup"><span data-stu-id="2f397-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="2f397-115">"Microsoft Graph" yra rekomenduojamas katalogo, tapatybės ir "Access" valdymo API.</span><span class="sxs-lookup"><span data-stu-id="2f397-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="2f397-116">Tačiau vis dar yra kelios spragos tarp to, kas įmanoma, "Azure AD Graph" ir "Microsoft Graph".</span><span class="sxs-lookup"><span data-stu-id="2f397-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="2f397-117">Peržiūrėkite šiuos straipsnius, kuriuose Akcentuokite naujausius skirtumus, kurie padės jums pasirinkti:</span><span class="sxs-lookup"><span data-stu-id="2f397-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="2f397-118">Išteklių tipo skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="2f397-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="2f397-119">Ypatybių skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"</span><span class="sxs-lookup"><span data-stu-id="2f397-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="2f397-120">"Azure AD" ir "Microsoft Graph" metodo skirtumai</span><span class="sxs-lookup"><span data-stu-id="2f397-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="2f397-121">**Kai gaunu užklausą dėl *vartotojo* objekto, daugelis jo ypatybių nėra**</span><span class="sxs-lookup"><span data-stu-id="2f397-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="2f397-122">`GET https://graph.microsoft.com/v1.0/users` pateikia tik 11 ypatybių, nes "Microsoft Graph" automatiškai parenka numatytąjį *vartotojų* ypatybių rinkinį.</span><span class="sxs-lookup"><span data-stu-id="2f397-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="2f397-123">Jei reikia kitų *vartotojo* ypatybių, naudokite $Select, kad pasirinktumėte programos poreikius.</span><span class="sxs-lookup"><span data-stu-id="2f397-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="2f397-124">Išbandykite **"Microsoft Graph Explorer"** pirmiausia.</span><span class="sxs-lookup"><span data-stu-id="2f397-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="2f397-125">**Kai kurios vartotojo ypatybių reikšmės yra *NULL* , nors žinau, kad jos nustatytos**</span><span class="sxs-lookup"><span data-stu-id="2f397-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="2f397-126">Greičiausiai paaiškinimas yra tas, kad taikomajai programai buvo suteiktas *vartotojas. ReadBasic. All* Permission.</span><span class="sxs-lookup"><span data-stu-id="2f397-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="2f397-127">Tai leidžia programai skaityti ribotą vartotojų ypatybių rinkinį, grąžinant visas kitas ypatybes kaip NULL, net jei jos buvo anksčiau nustatytos.</span><span class="sxs-lookup"><span data-stu-id="2f397-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="2f397-128">Bandykite suteikti taikomosios programos *vartotoją. skaityti. visi* teisės.</span><span class="sxs-lookup"><span data-stu-id="2f397-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="2f397-129">Daugiau informacijos ieškokite ["Microsoft Graph" vartotojų teisės](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="2f397-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="2f397-130">**Kyla problemų naudojant "OData" užklausos parametrus duomenims filtruoti pagal savo užklausas**</span><span class="sxs-lookup"><span data-stu-id="2f397-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="2f397-131">Nors "Microsoft Graph" palaiko platų "OData" užklausos parametrų intervalą, daugelis šių parametrų katalogų tarnybos nevisiškai palaiko (ištekliai, kurie paveldimi iš *Directoryobject*) programoje "Microsoft Graph".</span><span class="sxs-lookup"><span data-stu-id="2f397-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="2f397-132">Tie patys apribojimai, kurie buvo pateikti "Azure AD Graph", išlieka daugiausia programoje "Microsoft Graph":</span><span class="sxs-lookup"><span data-stu-id="2f397-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="2f397-133">**Nepalaikoma: $Count**, $search ir $Filter *NULL* arba *Not Null* reikšmės</span><span class="sxs-lookup"><span data-stu-id="2f397-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="2f397-134">**Nepalaikoma: $Filter** tam tikrų ypatybių (Peržiūrėkite išteklių temas, kuriose yra filtruojami ypatybės)</span><span class="sxs-lookup"><span data-stu-id="2f397-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="2f397-135">**Nepalaikoma: puslapių** kaita, filtravimas ir rūšiavimas vienu metu</span><span class="sxs-lookup"><span data-stu-id="2f397-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="2f397-136">**Nepalaikoma: ryšio** filtravimas.</span><span class="sxs-lookup"><span data-stu-id="2f397-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="2f397-137">Pavyzdžiui – raskite visus Jungtinės Karalystės inžinerijos grupės narius.</span><span class="sxs-lookup"><span data-stu-id="2f397-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="2f397-138">**Dalinis palaikymas**: $OrderBy *vartotojui* (tik DisplayName ir UserPrincipalName) ir *grupėje*</span><span class="sxs-lookup"><span data-stu-id="2f397-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="2f397-139">**Dalinis palaikymas**: $Filter (palaiko tik *EQ*, *Startswith*, *or* ir *and* *ir Limited)* palaikymą, $Expand (vieno objekto ryšių išplėtimas grąžina visus ryšius, bet objektų ryšių rinkinio išplėtimas yra ribotas)</span><span class="sxs-lookup"><span data-stu-id="2f397-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="2f397-140">Daugiau informacijos ieškokite [atsakymų su užklausos parametrais tinkinimas](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2f397-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="2f397-141">**Mano skambinimo API neveikia – kur galiu atlikti daugiau bandymų?**</span><span class="sxs-lookup"><span data-stu-id="2f397-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="2f397-142">**"Microsoft Graph Explorer"** – Išbandykite "Microsoft Graph" API savo nuomotojuje arba "demo" nuomotojuje, taip pat peržiūrėkite **užklausų užklausas** programoje "Microsoft Graph Explorer".</span><span class="sxs-lookup"><span data-stu-id="2f397-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="2f397-143">**Kai gaunu užklausą dėl duomenų, atrodo, kad gaunu neišsamią duomenų rinkinį**</span><span class="sxs-lookup"><span data-stu-id="2f397-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="2f397-144">Jei užklausiate rinkinį (pvz., *vartotojai*), "Microsoft Graph" naudoja serverio pusės puslapio apribojimus, todėl rezultatai visada grąžinami su numatytuoju puslapio dydžiu.</span><span class="sxs-lookup"><span data-stu-id="2f397-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="2f397-145">Jūsų programa visada turėtų tikėtis puslapio iš tarnybos grąžintų rinkinių.</span><span class="sxs-lookup"><span data-stu-id="2f397-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="2f397-146">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="2f397-146">For more information, see:</span></span>

- [<span data-ttu-id="2f397-147">"Microsoft Graph" geriausios praktikos</span><span class="sxs-lookup"><span data-stu-id="2f397-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="2f397-148">"Microsoft Graph" duomenų puslapių ieška taikomojoje programoje</span><span class="sxs-lookup"><span data-stu-id="2f397-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="2f397-149">**Mano programa yra per lėta ir taip pat yra Throttled. Kokius patobulinimus galiu padaryti?**</span><span class="sxs-lookup"><span data-stu-id="2f397-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="2f397-150">Atsižvelgiant į jūsų scenarijų, jūsų dispozicijoje yra įvairių įvairių parinkčių, kad jūsų programa būtų efektyvesnė, o kai kuriais atvejais mažiau būtų sulaikoma tarnyba (kai skambinate per daug kartų).</span><span class="sxs-lookup"><span data-stu-id="2f397-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="2f397-151">Jei norite sužinoti daugiau, žr.:</span><span class="sxs-lookup"><span data-stu-id="2f397-151">To learn more, see:</span></span>

- [<span data-ttu-id="2f397-152">"Microsoft Graph" geriausios praktikos</span><span class="sxs-lookup"><span data-stu-id="2f397-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="2f397-153">Užklausų grupavimas</span><span class="sxs-lookup"><span data-stu-id="2f397-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="2f397-154">Keitimų sekimas naudojant Delta užklausą</span><span class="sxs-lookup"><span data-stu-id="2f397-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="2f397-155">Gaukite pranešimus apie keitimą naudodami webkablius</span><span class="sxs-lookup"><span data-stu-id="2f397-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="2f397-156">Ribojimo gairės</span><span class="sxs-lookup"><span data-stu-id="2f397-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="2f397-157">**Kur galiu gauti daugiau informacijos apie klaidas ir žinomas problemas?**</span><span class="sxs-lookup"><span data-stu-id="2f397-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="2f397-158">"Microsoft Graph" klaidos atsakymo informacija</span><span class="sxs-lookup"><span data-stu-id="2f397-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="2f397-159">Žinomos "Microsoft Graph" problemos</span><span class="sxs-lookup"><span data-stu-id="2f397-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="2f397-160">**Kur galiu patikrinti paslaugų pasiekiamumo ir ryšio būseną?**</span><span class="sxs-lookup"><span data-stu-id="2f397-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="2f397-161">Tarnybų pasiekiamumo ir ryšio su pagrindinėmis tarnybomis, kurias galima pasiekti naudojant "Microsoft Graph", paslaugos gali turėti įtakos bendram "Microsoft Graph" pasiekiamumui ir veikimui.</span><span class="sxs-lookup"><span data-stu-id="2f397-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="2f397-162">"Azure Active Directory" tarnybos sveikatai patikrinkite **saugos + tapatybės** tarnybų būseną, išvardytas "Azure" [būsenos puslapyje](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="2f397-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="2f397-163">"Office" tarnyboms, kurios prisideda prie "Microsoft Graph", patikrinkite tarnybų, išvardintų " [Office" tarnybos sveikatos ataskaitų](https://portal.office.com/adminportal/home#/servicehealth)srityje, būseną.</span><span class="sxs-lookup"><span data-stu-id="2f397-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
