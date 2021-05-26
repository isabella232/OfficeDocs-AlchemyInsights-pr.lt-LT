---
title: Konfigūruokite galutinio punkto DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657937"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="55948-102">Konfigūruokite galutinio punkto DLP</span><span class="sxs-lookup"><span data-stu-id="55948-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="55948-103">„Microsoft“ galinio punkto DLP leidžia išplėsti DLP apsaugą ir stebėjimo galimybes iki slaptos informacijos „Windows 10“ įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="55948-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="55948-104">Kai įrenginiai parengti įrenginių valdymui, galite sukurti DLP strategijas, kad įgalintumėte elementų apsaugojimo veiksmus.</span><span class="sxs-lookup"><span data-stu-id="55948-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="55948-105">Veiklos naršyklę galima naudoti slaptų elementų veiklai stebėti.</span><span class="sxs-lookup"><span data-stu-id="55948-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="55948-106">Daugiau informacijos žr. [Įrenginių parengimas įrenginių valdymui](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="55948-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="55948-107">Norėdami pradėti naudoti galinio punkto DLP:</span><span class="sxs-lookup"><span data-stu-id="55948-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="55948-108">Įsitikinkite, kad turite atitinkamą SKU / prenumeratų licencijavimą.</span><span class="sxs-lookup"><span data-stu-id="55948-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="55948-109">Daugiau informacijos žr. [SKU / prenumeratų licencijavimas](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="55948-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="55948-110">Patikrinkite teises, reikalingas įrenginio valdymui įgalinti, prieigai prie parengimo puslapio arba įjungti / išjungti įrenginio stebėjimą.</span><span class="sxs-lookup"><span data-stu-id="55948-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="55948-111">Daugiau informacijos žr. [Teisės](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="55948-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="55948-112">Parenkite įrenginius įrenginių valdymui, laikantis įrenginių parengimo procedūros.</span><span class="sxs-lookup"><span data-stu-id="55948-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="55948-113">Daugiau informacijos žr. [Įrenginių parengimas](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="55948-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="55948-114">Sukurkite DLP strategiją, kad apsaugotumėte slaptus elementus.</span><span class="sxs-lookup"><span data-stu-id="55948-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="55948-115">Daugiau informacijos žr. [Galinio punkto DLP strategijos scenarijai](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="55948-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="55948-116">Daugiau informacijos apie „Microsoft“ galinio punkto DLP, žr. [Sužinokite apie „Microsoft 365“ galinio punkto duomenų praradimo prevenciją (peržiūra)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="55948-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="55948-117">**Svarbūs duomenų rinkimo veiksmai, jei reikia palaikymo:**</span><span class="sxs-lookup"><span data-stu-id="55948-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="55948-118">Atsisiųskite [MDATP kliento analizatoriaus peržiūrą.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="55948-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="55948-119">Paleiskite įrankį kaip administratorius iš cmd lango:</span><span class="sxs-lookup"><span data-stu-id="55948-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="55948-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="55948-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="55948-121">Kai būsite **paraginti Įvesti minučių skaičių,** kad būtų galima rinkti sekimą: įveskite minučių, reikalingų scenarijui vykdyti, skaičių.</span><span class="sxs-lookup"><span data-stu-id="55948-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="55948-122">Paleiskite scenarijų.</span><span class="sxs-lookup"><span data-stu-id="55948-122">Run the scenario.</span></span>

<span data-ttu-id="55948-123">Surinkite zip failo išvestį, kad ji būtų teikiama palaikymo agentui.</span><span class="sxs-lookup"><span data-stu-id="55948-123">Collect the Zip file output to give to the Support agent.</span></span>
