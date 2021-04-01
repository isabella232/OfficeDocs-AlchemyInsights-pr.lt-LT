---
title: „EndPoint Manager“ - saugos bazinės konfigūracijos
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440892"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="5a908-102">„EndPoint Manager“ - saugos bazinės konfigūracijos</span><span class="sxs-lookup"><span data-stu-id="5a908-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="5a908-103">Saugos bazinės konfigūracijos yra iš anksto sukonfigūruotos „Windows“ parametrų grupės, kurios padeda pritaikyti saugos parametrus, kuriuos rekomenduoja atitinkamos saugos komandos.</span><span class="sxs-lookup"><span data-stu-id="5a908-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="5a908-104">Šias bazines konfigūracijas galima tinkinti, kad būtų pateikti tik norimi parametrai ir vertės.</span><span class="sxs-lookup"><span data-stu-id="5a908-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="5a908-105">Norėdami gauti daugiau informacijos apie saugos bazines konfigūracijas, žr. [Saugos bazinių konfigūracijų naudojimas konfigūruojant „Windows 10“ įrenginius „Intune“](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="5a908-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="5a908-106">Šiuo metu yra šių produktų bazinės konfigūracijos:</span><span class="sxs-lookup"><span data-stu-id="5a908-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="5a908-107">„Windows MDM“ saugos parametrai</span><span class="sxs-lookup"><span data-stu-id="5a908-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="5a908-108">„Microsoft“ sargyba, skirta pabaigos taško saugai</span><span class="sxs-lookup"><span data-stu-id="5a908-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="5a908-109">„Microsoft Edge“</span><span class="sxs-lookup"><span data-stu-id="5a908-109">Microsoft Edge</span></span>

<span data-ttu-id="5a908-110">Kiekviena bazinė konfigūracija yra periodiškai atnaujinama ir išleidžiama palaipsniui.</span><span class="sxs-lookup"><span data-stu-id="5a908-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="5a908-111">Kiekviena versija įtraukia ir / arba pašalina ankstesnės versijos parametrus, kad būtų užtikrinta, jog bazinė konfigūracija atitinka dabartinius nurodymus.</span><span class="sxs-lookup"><span data-stu-id="5a908-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="5a908-112">Saugos bazinių konfigūracijų konsolė pabaigos taško saugoje leidžia palyginti skirtingas versijas, matant pakeitimus iš vienos versijos į kitą.</span><span class="sxs-lookup"><span data-stu-id="5a908-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="5a908-113">Dėl nurodymų, kaip efektyviausiai keisti diegiamą bazinės konfigūracijos versiją, žr. [ „Microsoft Intune“ saugos bazinės konfigūracijos tvarkymas](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="5a908-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="5a908-114">Pritaikę saugos bazinę konfigūraciją, galite stebėti diegimo būseną ir peržiūrėti parametrus kiekviename įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="5a908-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="5a908-115">**Pastaba:** bazinių konfigūracijų ataskaitų duomenys gali užtrukti iki 24 valandų, kol bus rodomos po pradinio diegimo įrenginyje, o iki tolesnių naujinimų - iki 6 valandų.</span><span class="sxs-lookup"><span data-stu-id="5a908-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="5a908-116">Dažniausia bazinės konfigūracijos parametro netaikymo priežastis yra ta, kad tas pats parametras naudojamas kitame profilyje.</span><span class="sxs-lookup"><span data-stu-id="5a908-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="5a908-117">Šį scenarijų galima ištirti konkrečiam įrenginiui, pasirinkus tą įrenginį iš įrenginio būsenos mazgo saugos bazinės konfigūracijos profilyje.</span><span class="sxs-lookup"><span data-stu-id="5a908-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="5a908-118">Daugiau informacijos žr. [Saugos bazinių konfigūracijų konfliktų sprendimas](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="5a908-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>