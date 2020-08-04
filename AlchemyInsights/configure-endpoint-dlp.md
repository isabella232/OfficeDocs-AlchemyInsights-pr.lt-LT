---
title: Konfigūruoti galinio punkto DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555555"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="e45df-102">Konfigūruoti galinio punkto DLP</span><span class="sxs-lookup"><span data-stu-id="e45df-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="e45df-103">"Microsoft Endpoint DLP" leidžia išplėsti DLP apsaugos ir stebėjimo galimybes slaptai informacijai "Windows 10" įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="e45df-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="e45df-104">Kai įrenginiai yra įtraukti į įrenginių valdymą, galite sukurti DLP strategijas, kad būtų galima įgalinti elementų apsaugos veiksmus.</span><span class="sxs-lookup"><span data-stu-id="e45df-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="e45df-105">Veiklos naršyklė gali būti naudojama stebėti veiklą jautriems elementams.</span><span class="sxs-lookup"><span data-stu-id="e45df-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="e45df-106">Daugiau informacijos rasite [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="e45df-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="e45df-107">Norėdami pradėti naudoti galinio punkto DLP:</span><span class="sxs-lookup"><span data-stu-id="e45df-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="e45df-108">Įsitikinkite, kad turite tinkamą SKU / prenumeratų licencijavimą.</span><span class="sxs-lookup"><span data-stu-id="e45df-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="e45df-109">Daugiau informacijos ieškokite [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="e45df-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="e45df-110">Patikrinkite teises, reikalingas įrenginių valdymui įgalinti, pasiekti parengimo puslapį arba įjungti / išjungti įrenginio stebėjimą.</span><span class="sxs-lookup"><span data-stu-id="e45df-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="e45df-111">Daugiau informacijos ieškokite [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="e45df-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="e45df-112">Borto įrenginius į įrenginių valdymą atlikdami borto įrenginių procedūrą.</span><span class="sxs-lookup"><span data-stu-id="e45df-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="e45df-113">Jei dalyje M365 atitikties **parametrai**trūksta parinkties Įrenginio parengimas (peržiūra), patvirtinkite, kad turite atitinkamą anksčiau nurodytą licenciją ir teises.</span><span class="sxs-lookup"><span data-stu-id="e45df-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="e45df-114">Daugiau informacijos rasite [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="e45df-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="e45df-115">Sukurkite DLP strategijas, kad apsaugotumėte savo jautrius elementus.</span><span class="sxs-lookup"><span data-stu-id="e45df-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="e45df-116">Informacijos ieškokite [Galinio punkto DLP strategijos scenarijai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="e45df-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="e45df-117">Daugiau informacijos apie "Microsoft Endpoint DLP" [ieškokite Sužinokite apie "Microsoft 365 Endpoint data loss prevention( preview)"](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="e45df-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>