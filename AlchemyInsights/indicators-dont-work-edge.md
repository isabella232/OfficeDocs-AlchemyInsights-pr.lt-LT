---
title: Indikatoriai neveikia naudojant "Edge" naršyklę
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676460"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="81f85-102">Indikatoriai neveikia naudojant "Edge" naršyklę</span><span class="sxs-lookup"><span data-stu-id="81f85-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="81f85-103">Sukūrus indikatorių, jo nepaiso "Edge" ("Smartscreen").</span><span class="sxs-lookup"><span data-stu-id="81f85-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="81f85-104">Daugiau informacijos žr. IP ir URL / [domenų indikatorių kūrimas.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="81f85-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="81f85-105">1 veiksmas: įsitikinkite, kad:</span><span class="sxs-lookup"><span data-stu-id="81f85-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="81f85-106">Patikrinkite, ar indikatorius teisingas (IP/URL nėra rašybos klaidų, teisingas veiksmas, tinkamos RBAC grupės).</span><span class="sxs-lookup"><span data-stu-id="81f85-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="81f85-107">Sukūrę indikatorių palaukite mažiausiai 2 valandas, kad būtų atsižvelgta į galimą gaišties laiką.</span><span class="sxs-lookup"><span data-stu-id="81f85-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="81f85-108">Įsitikinkite, kad sistema (-os) yra su "Microsoft" sargyba, skirta pabaigos taškui.</span><span class="sxs-lookup"><span data-stu-id="81f85-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="81f85-109">Patikrinkite, ar sistema (-os) gali bendrauti su debesimi.</span><span class="sxs-lookup"><span data-stu-id="81f85-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="81f85-110">Patikrinkite, ar "Smartscreen" įgalintas ir pasiekiamas nueię į [bandomąją svetainę.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="81f85-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="81f85-111">2 veiksmas: galimos problemos šalinimas</span><span class="sxs-lookup"><span data-stu-id="81f85-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="81f85-112">Įsitikinkite, kad klientas atitinka reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="81f85-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="81f85-113">Daugiau informacijos [žr. IP ir URL / domenų indikatorių kūrimas.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="81f85-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="81f85-114">Įsitikinkite, kad naudojate naujausią "Edge" naršyklės versiją.</span><span class="sxs-lookup"><span data-stu-id="81f85-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="81f85-115">Norėdami sužinoti naujausią versiją, [žr. Sužinokite, kurią Microsoft Edge versiją.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="81f85-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="81f85-116">Iš naujo paleiskite "Edge" naršyklę.</span><span class="sxs-lookup"><span data-stu-id="81f85-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="81f85-117">Eikite į svetainę, kurios indikatorių turite nustatyti.</span><span class="sxs-lookup"><span data-stu-id="81f85-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="81f85-118">Jei svetainė nerodoma taip, kaip tikėtasi, pereikite prie 3 veiksmo.</span><span class="sxs-lookup"><span data-stu-id="81f85-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="81f85-119">3 veiksmas: duomenų tvarkymas</span><span class="sxs-lookup"><span data-stu-id="81f85-119">Step 3: Collect data</span></span>

- <span data-ttu-id="81f85-120">Rinkti **MDEClientAnalyzer diagnostikos** duomenis.</span><span class="sxs-lookup"><span data-stu-id="81f85-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="81f85-121">Instrukcijas [žr. Problemos, susijusios su parengimo mašinomis "Microsoft Defender", skirta "Endpoint".](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="81f85-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="81f85-122">Jei jums patogu įdiegti ir rinkti "Fiddler" sekimą, žr. [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="81f85-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="81f85-123">Jei norite gauti patarimų iš "Microsoft" palaikymo tarnybą, pasirinkite toliau esančią palaikymo piktogramą, kad atidarytumėte palaikymo bylą.</span><span class="sxs-lookup"><span data-stu-id="81f85-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
