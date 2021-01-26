---
title: "\"Tokens\" problemos"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917040"
---
# <a name="issues-with-tokens"></a><span data-ttu-id="8032b-102">"Tokens" problemos</span><span class="sxs-lookup"><span data-stu-id="8032b-102">Issues with tokens</span></span>

<span data-ttu-id="8032b-103">Norėdami tvarkyti su atpažinimo ženklų problemas, galite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8032b-103">To manage issues related to tokens, you can perform the following steps:</span></span>

1. <span data-ttu-id="8032b-104">Galite apibrėžti "Microsoft" tapatybės platformos išduoto prieigos, ID arba SAML atpažinimo ženklo galiojimo laiką.</span><span class="sxs-lookup"><span data-stu-id="8032b-104">You can specify the lifetime of an access, ID, or SAML token issued by Microsoft identity platform.</span></span> <span data-ttu-id="8032b-105">Galite nustatyti atpažinimo ženklų naudojimo visas savo organizacijos taikomąsias programas, kelių nuomotojų (kelių organizacijų) taikomąją programą arba konkrečią organizacijos pagrindinę tarnybą.</span><span class="sxs-lookup"><span data-stu-id="8032b-105">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="8032b-106">Daugiau informacijos ieškokite ["Microsoft" tapatybės platformoje konfigūruojamų atpažinimo ženklų naudojimo laiko (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="8032b-106">For more information, see [Configurable token lifetimes in Microsoft identity platform (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="8032b-107">"Access" žetonai leidžia klientams saugiai skambinti apsaugotą žiniatinklio API ir juos naudoja žiniatinklio API, kad galėtų atlikti autentifikavimą ir autorizavimą.</span><span class="sxs-lookup"><span data-stu-id="8032b-107">Access tokens enable clients to securely call protected web APIs, and are used by web APIs to perform authentication and authorization.</span></span> <span data-ttu-id="8032b-108">Kaip ir OAuth specifikacija, "Access" žetonai yra nepermatomos eilutės, nenaudojant rinkinio formato – kai kurie tapatybės teikėjai (IDPs) naudoja GUID, kiti naudoja užšifruotą BLOB.</span><span class="sxs-lookup"><span data-stu-id="8032b-108">As per the OAuth specification, access tokens are opaque strings without a set format - some identity providers (IDPs) use GUIDs, others use encrypted blobs.</span></span> <span data-ttu-id="8032b-109">"Microsoft" tapatybės platformoje naudojami įvairūs "Access" atpažinimo ženklų formatai, atsižvelgiant į tai, kaip API konfigūracija priima atpažinimo ženklą.</span><span class="sxs-lookup"><span data-stu-id="8032b-109">The Microsoft identity platform uses a variety of access token formats, depending on the configuration of the API that accepts the token.</span></span> <span data-ttu-id="8032b-110">Norėdami sužinoti, kaip jūsų API gali patvirtinti ir naudoti "Access" atpažinimo ženklo teiginius, peržiūrėkite ["Microsoft" tapatybės platformos prieigos žetonus](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).</span><span class="sxs-lookup"><span data-stu-id="8032b-110">To learn how your API can validate and use the claims inside an access token, see [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).</span></span>
3. <span data-ttu-id="8032b-111">"Microsoft" autentifikavimo biblioteka (MSAL) palaiko kelis autentifikavimo srautus, skirtus naudoti skirtinguose taikomosios programos scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="8032b-111">The Microsoft Authentication Library (MSAL) supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="8032b-112">Daugiau informacijos ieškokite [autentifikavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).</span><span class="sxs-lookup"><span data-stu-id="8032b-112">For more information, see [Authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).</span></span>
4. <span data-ttu-id="8032b-113">"OAuth 2,0" autorizavimo kodo dotaciją galima naudoti įrenginyje įdiegtose programėlėse, norint gauti prieigą prie apsaugotų išteklių, pvz., žiniatinklio API.</span><span class="sxs-lookup"><span data-stu-id="8032b-113">The OAuth 2.0 authorization code grant can be used in apps that are installed on a device to gain access to protected resources, such as web APIs.</span></span> <span data-ttu-id="8032b-114">Naudodami "Microsoft" tapatybės platformos "OAuth 2,0" diegimą, galite įtraukti prisijungimo ir API prieigą prie mobiliųjų įrenginių ir kompiuterio taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="8032b-114">Using the Microsoft identity platform implementation of OAuth 2.0, you can add sign-in and API access to your mobile and desktop apps.</span></span> <span data-ttu-id="8032b-115">Peržiūrėkite ["Microsoft" tapatybės platformą ir "OAuth" 2,0 autorizavimo kodo srautą](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) , kaip tiesiogiai programos protokolą programoje, naudojant bet kurią kalbą.</span><span class="sxs-lookup"><span data-stu-id="8032b-115">See [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) for how to program directly against the protocol in your application, using any language.</span></span>
5. <span data-ttu-id="8032b-116">OpenID Connect (OIDC) yra autentifikavimo protokolas, sukurtas "OAuth 2,0", kurį galite naudoti norėdami saugiai prisijungti vartotojui į taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="8032b-116">OpenID Connect (OIDC) is an authentication protocol built on OAuth 2.0 that you can use to securely sign in a user to an application.</span></span> <span data-ttu-id="8032b-117">Kai naudojate "Microsoft" tapatybės platformos galinio punkto "OpenID Connect" įdiegtį, galite įtraukti prisijungimo ir API prieigą prie savo taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="8032b-117">When you use the Microsoft identity platform endpoint's implementation of OpenID Connect, you can add sign-in and API access to your apps.</span></span> <span data-ttu-id="8032b-118">Naudojant ["Microsoft" tapatybės platformą ir "OpenID Connect" protokolą](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) rodoma, kaip tai padaryti nepriklausomai nuo kalbos ir aprašoma, kaip siųsti ir gauti http pranešimą nenaudojant jokių "Microsoft" atvirosios šaltinio bibliotekų.</span><span class="sxs-lookup"><span data-stu-id="8032b-118">[Microsoft identity platform and OpenID Connect protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) shows how to do this independent of language and describes how to send and receive HTTP messages without using any Microsoft open-source libraries.</span></span>
    - <span data-ttu-id="8032b-119">UserInfo galinis punktas yra OIDC standarto dalis, skirta pateikti teiginius apie autentifikuotą vartotoją.</span><span class="sxs-lookup"><span data-stu-id="8032b-119">The UserInfo endpoint is part of the OIDC standard, designed to return claims about the user that authenticated.</span></span> <span data-ttu-id="8032b-120">Daugiau informacijos ieškokite ["Microsoft" tapatybės platformos UserInfo galinio punkto](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).</span><span class="sxs-lookup"><span data-stu-id="8032b-120">For more information, see [Microsoft identity platform UserInfo endpoint](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).</span></span>
    - <span data-ttu-id="8032b-121">Žiniatinklio taikomosios programos [Skambinimas žiniatinklio API naudojant "AZURE AD" ir "OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) " pavyzdys rodo, kaip kurti MVC žiniatinklio taikomąją programą, kuri naudoja "Azure AD" prisijungimui naudodami "OpenID Connect" protokolą, o tada paskambinti žiniatinklio API pagal vartotojo tapatybę, naudodami atpažinimo ženklus, gautus naudojant "oauth 2,0".</span><span class="sxs-lookup"><span data-stu-id="8032b-121">The [Calling a web API in a web app using Azure AD and OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) sample shows how to build an MVC web application that uses Azure AD for sign-in using the OpenID Connect protocol, and then call a web API under the signed-in user's identity using tokens obtained via OAuth 2.0.</span></span> <span data-ttu-id="8032b-122">Šis pavyzdys naudoja OpenID Connect ASP .net OWIN tarpinės ir adal .net.</span><span class="sxs-lookup"><span data-stu-id="8032b-122">This sample uses the OpenID Connect ASP .Net OWIN middleware and ADAL .Net.</span></span>
6. <span data-ttu-id="8032b-123">[Konfigūruokite taikomąją programą, kad būtų galima atskleisti žiniatinklio API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – šiame "QuickStart" užregistruojate žiniatinklio API naudodami "Microsoft" tapatybės platformą ir įtraukite ją į kliento taikomąsias programas įtraukdami pavyzdžio aprėptį.</span><span class="sxs-lookup"><span data-stu-id="8032b-123">[Configure an application to expose a web API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - In this quickstart, you register a web API with the Microsoft identity platform and expose it to client apps by adding an example scope.</span></span> <span data-ttu-id="8032b-124">Registruodami žiniatinklio API ir naudodami aprėptis, galite suteikti teisėmis pagrįstą prieigą prie jos išteklių įgaliotiems vartotojams ir kliento programoms, kurios pasiekia jūsų API.</span><span class="sxs-lookup"><span data-stu-id="8032b-124">By registering your web API and exposing it through scopes, you can provide permissions-based access to its resources to authorized users and client apps that access your API.</span></span>
7. <span data-ttu-id="8032b-125">"Azure Active Directory" B2C ("Azure AD B2C") išteklių savininko slaptažodžio kredencialus (ROPC) srautas yra OAuth Standard autentifikavimo srautas.</span><span class="sxs-lookup"><span data-stu-id="8032b-125">In Azure Active Directory B2C (Azure AD B2C), the resource owner password credentials (ROPC) flow is an OAuth standard authentication flow.</span></span> <span data-ttu-id="8032b-126">Šiame sraute taikomoji programa, taip pat žinoma kaip besiremianti šalis, leidžia naudoti "Tokens" leistinus kredencialus.</span><span class="sxs-lookup"><span data-stu-id="8032b-126">In this flow, an application, also known as the relying party, exchanges valid credentials for tokens.</span></span> <span data-ttu-id="8032b-127">Kredencialai apima vartotojo ID ir slaptažodį.</span><span class="sxs-lookup"><span data-stu-id="8032b-127">The credentials include a user ID and password.</span></span> <span data-ttu-id="8032b-128">Pateikti žetonai yra ID atpažinimo ženklas, prieigos žetonas ir atnaujinimo atpažinimo ženklas.</span><span class="sxs-lookup"><span data-stu-id="8032b-128">The tokens returned are an ID token, access token, and a refresh token.</span></span> <span data-ttu-id="8032b-129">Daugiau informacijos ieškokite [išteklių savininko slaptažodžio kredencialų srauto nustatymas "Azure Active Directory" B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="8032b-129">For more information, see [Set up a resource owner password credentials flow in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow).</span></span> 
