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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402440"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="7cad7-102">Konfigūruokite galutinio punkto DLP</span><span class="sxs-lookup"><span data-stu-id="7cad7-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="7cad7-103">„Microsoft“ galinio punkto DLP leidžia išplėsti DLP apsaugą ir stebėjimo galimybes iki slaptos informacijos „Windows 10“ įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="7cad7-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="7cad7-104">Kai įrenginiai parengti įrenginių valdymui, galite sukurti DLP strategijas, kad įgalintumėte elementų apsaugojimo veiksmus.</span><span class="sxs-lookup"><span data-stu-id="7cad7-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="7cad7-105">Veiklos naršyklę galima naudoti slaptų elementų veiklai stebėti.</span><span class="sxs-lookup"><span data-stu-id="7cad7-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="7cad7-106">Daugiau informacijos žr. [Įrenginių parengimas įrenginių valdymui](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="7cad7-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="7cad7-107">Norėdami pradėti naudoti galinio punkto DLP:</span><span class="sxs-lookup"><span data-stu-id="7cad7-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="7cad7-108">Įsitikinkite, kad turite atitinkamą SKU / prenumeratų licencijavimą.</span><span class="sxs-lookup"><span data-stu-id="7cad7-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="7cad7-109">Daugiau informacijos žr. [SKU / prenumeratų licencijavimas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="7cad7-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="7cad7-110">Patikrinkite teises, reikalingas įrenginio valdymui įgalinti, prieigai prie parengimo puslapio arba įjungti / išjungti įrenginio stebėjimą.</span><span class="sxs-lookup"><span data-stu-id="7cad7-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="7cad7-111">Daugiau informacijos žr. [Teisės](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="7cad7-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="7cad7-112">Parenkite įrenginius įrenginių valdymui, laikantis įrenginių parengimo procedūros.</span><span class="sxs-lookup"><span data-stu-id="7cad7-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="7cad7-113">Jei trūksta parinkties „Įrenginio parengimas“ (peržiūra), esančios „M365“ atitikties  **parametruose**, įsitikinkite, kad turite tinkamą anksčiau nurodytą licenciją ir teises.</span><span class="sxs-lookup"><span data-stu-id="7cad7-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="7cad7-114">Daugiau informacijos žr. [Įrenginių parengimas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="7cad7-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="7cad7-115">Sukurkite DLP strategiją, kad apsaugotumėte slaptus elementus.</span><span class="sxs-lookup"><span data-stu-id="7cad7-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="7cad7-116">Daugiau informacijos žr. [Galinio punkto DLP strategijos scenarijai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7cad7-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="7cad7-117">Daugiau informacijos apie „Microsoft“ galinio punkto DLP, žr. [Sužinokite apie „Microsoft 365“ galinio punkto duomenų praradimo prevenciją (peržiūra)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="7cad7-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="7cad7-118">**Svarbūs duomenų rinkimo veiksmai, jei reikia palaikymo:**</span><span class="sxs-lookup"><span data-stu-id="7cad7-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="7cad7-119">Atsisiųskite MDATP kliento analizatoriaus peržiūros versiją iš [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="7cad7-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="7cad7-120">Paleiskite įrankį kaip administratorius iš cmd lango:</span><span class="sxs-lookup"><span data-stu-id="7cad7-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="7cad7-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="7cad7-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="7cad7-122">Kai būsite paraginti „Įveskite sekimų rinkimo minučių skaičių: “, įveskite minučių skaičių, reikalingą scenarijui paleisti</span><span class="sxs-lookup"><span data-stu-id="7cad7-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="7cad7-123">Paleisti scenarijų</span><span class="sxs-lookup"><span data-stu-id="7cad7-123">Run the scenario</span></span>

<span data-ttu-id="7cad7-124">Surinkite „Zip“ failo išvestį, kuri bus pateikta palaikymo agentui.</span><span class="sxs-lookup"><span data-stu-id="7cad7-124">Collect the Zip file output to be given to the Support agent.</span></span>
