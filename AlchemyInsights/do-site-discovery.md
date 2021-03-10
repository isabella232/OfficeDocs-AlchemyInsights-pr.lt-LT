---
title: Svetainių aptikimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693483"
---
# <a name="do-site-discovery"></a><span data-ttu-id="922ad-102">Svetainių aptikimas</span><span class="sxs-lookup"><span data-stu-id="922ad-102">Do site discovery</span></span>

<span data-ttu-id="922ad-103">Jei jūsų organizacija vis dar naudoja senstelėjusias žiniatinklio programas ir planus naudoti "Internet Explorer" režimą (kurį dauguma klientų), tada reikia atlikti kai kuriuos papildomus svetainių atradimus.</span><span class="sxs-lookup"><span data-stu-id="922ad-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="922ad-104">**Jau įdiegėte senesnę "Microsoft Edge" versiją**</span><span class="sxs-lookup"><span data-stu-id="922ad-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="922ad-105">Jei jau sukonfigūravote savo įmonės svetainių sąrašą, kad galėtumėte dirbti su senesnė "Microsoft Edge" versija, jūsų svetainės aptikimas beveik baigtas.</span><span class="sxs-lookup"><span data-stu-id="922ad-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="922ad-106">Reikia įtraukti neutralias svetaines.</span><span class="sxs-lookup"><span data-stu-id="922ad-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="922ad-107">Neutralios svetainės paprastai yra svetainės, kurios teikia bendrąją autentifikacija (SSO).</span><span class="sxs-lookup"><span data-stu-id="922ad-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="922ad-108">Jei einate į neutralią svetainę iš "Microsoft Edge", "Microsoft Edge" norite pasilikti, kad autentifikuotumėte.</span><span class="sxs-lookup"><span data-stu-id="922ad-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="922ad-109">Jei einate į neutralią svetainę programoje "Internet Explorer", tada norite sustabdyti "Internet Explorer" režimą, kad autentifikuotumėte.</span><span class="sxs-lookup"><span data-stu-id="922ad-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="922ad-110">Identifikuokite bet kokias SSO arba kitas neutralias svetaines ir įtraukite jas į savo įmonės svetainių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="922ad-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="922ad-111">**"Internet Explorer" yra jūsų numatytoji naršyklė**</span><span class="sxs-lookup"><span data-stu-id="922ad-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="922ad-112">Jei dabar naudojate tik "Internet Explorer", jums gali nežinoti, kurios svetainės buvo atnaujintos į šiuolaikinius žiniatinklio standartus ir kurioms vis dar reikia "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="922ad-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="922ad-113">Norite surasti ir įtraukti šias svetaines į įmonės svetainių sąrašą, kad galėtumėte naudoti "Internet Explorer" režimą tik tose svetainėse.</span><span class="sxs-lookup"><span data-stu-id="922ad-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="922ad-114">[Įmonės svetainės aptikimas](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) aptinka svetaines, kurioms gali reikėti "Internet Explorer" režimo.</span><span class="sxs-lookup"><span data-stu-id="922ad-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="922ad-115">Galima rinkti duomenis kompiuteriuose, kuriuose veikia "Windows Internet Explorer 8", naudojant "Internet Explorer 11" sistemoje "Windows 10", "Windows 8,1" arba "Windows 7".</span><span class="sxs-lookup"><span data-stu-id="922ad-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="922ad-116">**Duomenų analizė**</span><span class="sxs-lookup"><span data-stu-id="922ad-116">**Analyze the data**</span></span>

<span data-ttu-id="922ad-117">Surinkę svetainių duomenis rekomenduojame atlikti šiuos keturių etapų procesus, kad galėtumėte analizuoti duomenis:</span><span class="sxs-lookup"><span data-stu-id="922ad-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="922ad-118">Rūšiuokite duomenis pagal domeną, tada pagal URL.</span><span class="sxs-lookup"><span data-stu-id="922ad-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="922ad-119">Apibrėžkite taikomosios programos ribas, kad sukonfigūruotumėte "Internet Explorer" režimą.</span><span class="sxs-lookup"><span data-stu-id="922ad-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="922ad-120">Norite įtraukti visas svetaines ir žiniatinklio valdiklius, kurie apibrėžia programėlę, bet nenorite įtraukti papildomų svetainių ir valdiklių.</span><span class="sxs-lookup"><span data-stu-id="922ad-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="922ad-121">Kai kurios svetainės gali būti taip paprastos, kaip *https://contoso.com/app1* tuo metu, kai kitos gali reikalauti apibrėžti kelias svetaines ir puslapius.</span><span class="sxs-lookup"><span data-stu-id="922ad-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="922ad-122">Išbandykite taikomąją programą, kad įsitikintumėte, jog ji neveikia gimtoji.</span><span class="sxs-lookup"><span data-stu-id="922ad-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="922ad-123">Daugelis svetainių pasiūlys šiuolaikinį turinį, kai aptiks šiuolaikinę naršyklę ir pasiūlys tik senstelėjusį turinį, kai aptiks "Internet Explorer".</span><span class="sxs-lookup"><span data-stu-id="922ad-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="922ad-124">Įtraukite taikomąją programą į savo įmonės svetainių sąrašą, jei ji nepateikia bandymų.</span><span class="sxs-lookup"><span data-stu-id="922ad-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="922ad-125">Geriausia praktika – grupuoti visas svetaines, kurios susideda iš programos.</span><span class="sxs-lookup"><span data-stu-id="922ad-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="922ad-126">Tokiu būdu naujinant taikomąją programą lengviau pašalinti visą svetainę iš "Internet Explorer" režimo ir pradėti naudoti šiuolaikinę tos programos naršyklę.</span><span class="sxs-lookup"><span data-stu-id="922ad-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="922ad-127">Kai atliksite svetainių atradimą ir išanalizavote duomenis, esate pasirengę pradėti ieškoti kanalo strategijos.</span><span class="sxs-lookup"><span data-stu-id="922ad-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

