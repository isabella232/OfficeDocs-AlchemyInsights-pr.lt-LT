---
title: EndPoint Manager – saugos bazinės linijos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421084"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="154e6-102">EndPoint Manager – saugos bazinės linijos</span><span class="sxs-lookup"><span data-stu-id="154e6-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="154e6-103">Saugos bazinės linijos yra iš anksto sukonfigūruotos "Windows" parametrų grupės, kurios padeda taikyti saugos parametrus, rekomenduojamus atitinkamų saugos komandų.</span><span class="sxs-lookup"><span data-stu-id="154e6-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="154e6-104">Šias bazines linijas galima tinkinti, kad būtų pateikti tik norimi parametrai ir reikšmės.</span><span class="sxs-lookup"><span data-stu-id="154e6-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="154e6-105">Daugiau informacijos apie saugos bazines linijas žr. Saugos bazinės linijos naudojimas ["Windows 10" įrenginiams konfigūruoti "Intune".](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="154e6-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="154e6-106">Šiuo metu yra šių produktų bazinės linijos:</span><span class="sxs-lookup"><span data-stu-id="154e6-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="154e6-107">"Windows MDM" saugos parametrai</span><span class="sxs-lookup"><span data-stu-id="154e6-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="154e6-108">"Microsoft" sargyba, skirta "EndPoint" saugos</span><span class="sxs-lookup"><span data-stu-id="154e6-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="154e6-109">„Microsoft Edge“</span><span class="sxs-lookup"><span data-stu-id="154e6-109">Microsoft Edge</span></span>

<span data-ttu-id="154e6-110">Kiekviena bazinė informacija periodiškai atnaujinama ir išleidžiama papildomose versijose.</span><span class="sxs-lookup"><span data-stu-id="154e6-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="154e6-111">Kiekviena versija įtraukia ir pašalina ankstesnės versijos parametrus, kad įsitikintų, jog bazinė linija atitinka dabartines rekomendacijas.</span><span class="sxs-lookup"><span data-stu-id="154e6-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="154e6-112">"Endpoint Security" bazinės saugos konsolė leidžia palyginti skirtingas versijas, nes pakeitimai iš versijos į versiją matomi.</span><span class="sxs-lookup"><span data-stu-id="154e6-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="154e6-113">Patarimų, kaip efektyviausiai pakeisti bazinės linijos versiją, [žr. "Microsoft Intune" saugos bazinių linijų profilių valdymas.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="154e6-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="154e6-114">Įdiegę saugos bazinę liniją, galite stebėti diegimo būseną ir peržiūrėti parametrus pagal įrenginį.</span><span class="sxs-lookup"><span data-stu-id="154e6-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="154e6-115">**Pastaba:** Bazinės linijos ataskaitų duomenys gali užtrukti iki 24 valandų, kad jie būtų rodomi nuo pradinio diegimo prie įrenginio ir iki 6 valandų, kad būtų galima atlikti tolesnius naujinimus.</span><span class="sxs-lookup"><span data-stu-id="154e6-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="154e6-116">Dažniausia bazinės linijos parametro taikymo priežastis yra ta, kad tas pats parametras naudojamas skirtinguose profiliuose.</span><span class="sxs-lookup"><span data-stu-id="154e6-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="154e6-117">Šį scenarijų galima ištirti konkrečiam įrenginiui pasirinkus tą įrenginį saugos bazinės linijos profilio mazge Įrenginio būsena.</span><span class="sxs-lookup"><span data-stu-id="154e6-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="154e6-118">Daugiau informacijos [žr. Saugos bazinių duomenų konfliktų sprendimas.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="154e6-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>