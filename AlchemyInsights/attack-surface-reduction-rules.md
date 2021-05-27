---
title: Atakos paviršiaus mažinimo taisyklės
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676436"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c2d28-102">Atakos paviršiaus mažinimo taisyklės</span><span class="sxs-lookup"><span data-stu-id="c2d28-102">Attack surface reduction rules</span></span>

<span data-ttu-id="c2d28-103">Neįtraukus failų ar aplankų, gali labai sumažėti apsauga, kurią teikia atakos paviršiaus mažinimo taisyklės.</span><span class="sxs-lookup"><span data-stu-id="c2d28-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="c2d28-104">Failai, kuriuos blokavo taisyklė, leidžiami vykdyti, o ataskaita ar įvykis neįrašomi.</span><span class="sxs-lookup"><span data-stu-id="c2d28-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="c2d28-105">Išimtis taikoma visoms taisyklėms, kurios leidžia išimtis.</span><span class="sxs-lookup"><span data-stu-id="c2d28-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="c2d28-106">ASR išimtys naudoja tą pačią sintaksę kaip "Microsoft" sargybos antivirusinė programa išimtys.</span><span class="sxs-lookup"><span data-stu-id="c2d28-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="c2d28-107">Išsamesnės informacijos ieškokite ""Microsoft" sargybos antivirusinė programa" išimčių [konfigūravimas ir "Microsoft" sargybos antivirusinė programa.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c2d28-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="c2d28-108">Norėdami išvengti problemų, peržiūrėkite [Dažnai pasitaikančių klaidų, kad išvengtumėte apibrėždami išimtis](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="c2d28-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c2d28-109">Ne visos ASR taisyklės palaiko išimtis.</span><span class="sxs-lookup"><span data-stu-id="c2d28-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="c2d28-110">Norėdami patikrinti, ar jūsų taisyklė palaiko išimtis, žr. lentelę [Atakos paviršiaus mažinimo taisyklės](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="c2d28-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c2d28-111">Atakos paviršiaus mažinimo taisyklės</span><span class="sxs-lookup"><span data-stu-id="c2d28-111">Attack surface reduction rules</span></span>

<span data-ttu-id="c2d28-112">Jūsų organizacijos atakos paviršius apima visas vietas, kuriose pažeidėjas gali pakenkti organizacijos įrenginiams ar tinklams.</span><span class="sxs-lookup"><span data-stu-id="c2d28-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="c2d28-113">Atakos paviršiaus mažinimas reiškia organizacijos įrenginių ir tinklo apsaugą, todėl puolama mažiau būdų, kaip atlikti atakas.</span><span class="sxs-lookup"><span data-stu-id="c2d28-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="c2d28-114">Gali padėti "Microsoft" sargybos galinio punkto atakos paviršiaus mažinimo taisyklių konfigūravimas.</span><span class="sxs-lookup"><span data-stu-id="c2d28-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="c2d28-115">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="c2d28-115">For more information, see:</span></span>

- [<span data-ttu-id="c2d28-116">Susieti ASR taisyklės GUID pavadinimą</span><span class="sxs-lookup"><span data-stu-id="c2d28-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="c2d28-117">ASR taisyklių reikalavimai:</span><span class="sxs-lookup"><span data-stu-id="c2d28-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="c2d28-118">Windows 10 Pro 1709 arba naujesnė versija</span><span class="sxs-lookup"><span data-stu-id="c2d28-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c2d28-119">Windows 10 Enterprise 1709 arba naujesnė versija</span><span class="sxs-lookup"><span data-stu-id="c2d28-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c2d28-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span><span class="sxs-lookup"><span data-stu-id="c2d28-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="c2d28-121">Tinkamos taikyti išimties identifikas</span><span class="sxs-lookup"><span data-stu-id="c2d28-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="c2d28-122">"Microsoft-Windows-"Windows" sargyba" žurnale ieškokite įvykio ID 1121 arba 1122.</span><span class="sxs-lookup"><span data-stu-id="c2d28-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="c2d28-123">Įvertinkite blokavimo scenarijų ir kontekstą ir patvirtinkite, kad šis scenarijus turi būti atblokuotas.</span><span class="sxs-lookup"><span data-stu-id="c2d28-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="c2d28-124">Įvykio išsamioje dalyje perskaitykite reikšmę Kelias, kuri yra reikšmę, kuri apibrėžia išimtį.</span><span class="sxs-lookup"><span data-stu-id="c2d28-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="c2d28-125">Padarykite, kad išimtis būtų kuo griežtesnė.</span><span class="sxs-lookup"><span data-stu-id="c2d28-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="c2d28-126">Prireikus pritaikykite pakaitos simbolį (pvz., pakeiskite vartotojo kintamąjį).</span><span class="sxs-lookup"><span data-stu-id="c2d28-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="c2d28-127">Taikyti išimtį pagal savo diegimo poreikius.</span><span class="sxs-lookup"><span data-stu-id="c2d28-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="c2d28-128">Daugiau informacijos žr. [Atakos paviršiaus mažinimo taisyklių tinkinimas.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="c2d28-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="c2d28-129">Išimtis nepaiso</span><span class="sxs-lookup"><span data-stu-id="c2d28-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="c2d28-130">Nustatykite, ar taisyklė palaiko išimtis.</span><span class="sxs-lookup"><span data-stu-id="c2d28-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="c2d28-131">Daugiau informacijos žr. [Atakos paviršiaus mažinimo taisyklės](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="c2d28-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="c2d28-132">Peržiūrėkite taikomas išimtis ir patikrinkite naudodami rašybos klaidų arba klaidingai interpretuotos pakaitos simbolių įvykio duomenis.</span><span class="sxs-lookup"><span data-stu-id="c2d28-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="c2d28-133">Daugiau informacijos žr. [Palaikomi išimčių tipai](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="c2d28-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="c2d28-134">jei taisyklės poveikis per didelis, apsvarstykite galimybę perkelti taisyklę (atgal) į audito režimą, kad būtų galima atlikti tolesnį tikrinimą.</span><span class="sxs-lookup"><span data-stu-id="c2d28-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="c2d28-135">Daugiau informacijos žr. [Tikrinimas, kaip "Microsoft" sargyba galinių punktų funkcijoms veikia audito režimu](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="c2d28-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="c2d28-136">Norėdami atidaryti palaikymo atvejį, rinkite palaikymo duomenis naudodami šią komandą:</span><span class="sxs-lookup"><span data-stu-id="c2d28-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="c2d28-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="c2d28-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="c2d28-138">Daugiau informacijos žr. ["Microsoft" sargybos galinių punktų parengimo įrenginių problemos.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="c2d28-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
