---
title: Saitų ir URL problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707890"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="bfae2-102">Saitų ir URL problemos</span><span class="sxs-lookup"><span data-stu-id="bfae2-102">Issues with links and URLs</span></span>

<span data-ttu-id="bfae2-103">Peradresavimo URI / atsakymo URL (abu terminai gali būti naudojami pakaitomis) – tai URL, kuriuos naudoja „Microsoft“ tapatybės platforma, kad pateiktų programos prašomus atpažinimo ženklus.</span><span class="sxs-lookup"><span data-stu-id="bfae2-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="bfae2-104">Daugiau informacijos apie šiuos URL žr. toliau pateiktuose straipsniuose:</span><span class="sxs-lookup"><span data-stu-id="bfae2-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="bfae2-105">[Autentifikavimo srautai ir programų scenarijai](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacija apie peradresavimo URI **programos registracijos** puslapyje kiekvienam scenarijui.</span><span class="sxs-lookup"><span data-stu-id="bfae2-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="bfae2-106">Peradresavimo URI / atsakymo URL apribojimai</span><span class="sxs-lookup"><span data-stu-id="bfae2-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="bfae2-107">**Nežinau, kaip užregistruoti tinkamą peradresavimo URI / atsakymo URL**</span><span class="sxs-lookup"><span data-stu-id="bfae2-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="bfae2-108">Kai prisijungiate naudodami programą, kurią kuriate, jeigu prisijungimo dialogo langas rodo **AADSTS50011: Prašyme nurodytas url neatitinka url sukonfigūruotų šiai programai <your app ID>**, turėsite įtraukti programos registraciją, peradresavimo URI, kurį naudojo jūsų kodas atpažinimo ženklo prašyme „Microsoft“ tapatybės platformai.</span><span class="sxs-lookup"><span data-stu-id="bfae2-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="bfae2-109">Norėdami įtraukti atsakymo URL, eikite į skirtuką **Autentifikavimas**, esantį jūsų **programos registracijos** puslapyje „Azure“ portale ir įtraukite įrašą dalyje **Peradresavimo URI**.</span><span class="sxs-lookup"><span data-stu-id="bfae2-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="bfae2-110">Reikšmė, kurią turite įvesti, priklauso nuo programos, kurią kuriate, tipo, kaip aprašyta žemiau:</span><span class="sxs-lookup"><span data-stu-id="bfae2-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="bfae2-111">Vieno puslapio programų ir žiniatinklio programų atveju atsakymo URL yra jūsų programos URL.</span><span class="sxs-lookup"><span data-stu-id="bfae2-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="bfae2-112">Žr. [vieno puslapio programos registracija](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) arba [žiniatinklio programos registracija naudojant „Azure“ portalą](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="bfae2-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="bfae2-113">Darbalaukio programoms, reikšmė, kurią turite pasirinkti priklauso nuo:</span><span class="sxs-lookup"><span data-stu-id="bfae2-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="bfae2-114">platformos („MacOS“ skiriasi nuo „Windows“ arba „Linux“)</span><span class="sxs-lookup"><span data-stu-id="bfae2-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="bfae2-115">to, kaip gaunate atpažinimo ženklą (interkatyviai, su įrenginio kodų srautu, su integruotuoju „Windows“ autentifikavimu [IWA] arba su vartotojo vardu / slaptažodžiu).</span><span class="sxs-lookup"><span data-stu-id="bfae2-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="bfae2-116">Daugiau informacijos žr. [darbalaukio programos – programų registracija – peradresavimo URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="bfae2-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="bfae2-117">Mobiliųjų įrenginių programose peradresavimo URI priklauso nuo:</span><span class="sxs-lookup"><span data-stu-id="bfae2-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="bfae2-118">platformos („iOS“ / „Android“ / „UWP“)</span><span class="sxs-lookup"><span data-stu-id="bfae2-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="bfae2-119">informacijos, kuri buvo naudojama kuriant jūsų programą, pvz., „iOS“ grupavimo ID bei „Android“ paketo pavadinimo ir parašo maišos. „Azure“ portalo registracijos programa jums padės.</span><span class="sxs-lookup"><span data-stu-id="bfae2-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="bfae2-120">Daugiau informacijos žr. [platformos konfigūravimas ir peradresavimo URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="bfae2-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="bfae2-121">Žiniatinklio API ir kai kurie iš automatinių atpažinimo ženklų gavimo būdų (IWA ir vartotojo vardas / slaptažodis) nereikalauja peradresavimo URI.</span><span class="sxs-lookup"><span data-stu-id="bfae2-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="bfae2-122">**Įdiegiau savo žiniatinklio programą, o kai bandau ją patikrinti, gaunu atsakymo URL neatitikimo pranešimą**</span><span class="sxs-lookup"><span data-stu-id="bfae2-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="bfae2-123">Įtraukite peradresavimo URI visose vietose, kuriose diegiate žiniatinklio programą.</span><span class="sxs-lookup"><span data-stu-id="bfae2-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="bfae2-124">Daugiau informacijos žr. [Registruokite žiniatinklio programos programą naudodami „Azure“ portalą](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="bfae2-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="bfae2-125">Įtraukite peradresavimo URI į vietą iškart po to, kai įdiegsite programą toje vietoje.</span><span class="sxs-lookup"><span data-stu-id="bfae2-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="bfae2-126">**Negaliu užregistruoti pakankamai atsakymo URL**</span><span class="sxs-lookup"><span data-stu-id="bfae2-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="bfae2-127">Esate ISV ir turite vieną ar kelis peradresavimo URI kiekvienam savo klientui.</span><span class="sxs-lookup"><span data-stu-id="bfae2-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="bfae2-128">Norite perkelti iš ADAL / „Azure AD“ v1.0 į MSAL / „Microsoft“ tapatybės platformą ir pasirodo pranešimas [maksimalus peradresavimo URI skaičius](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="bfae2-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="bfae2-129">Norėdami išspręsti šią problemą, [įtraukite peradresavimo URI į paslaugų principus](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) kurie atitinka kiekvieną iš jūsų klientų.</span><span class="sxs-lookup"><span data-stu-id="bfae2-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
