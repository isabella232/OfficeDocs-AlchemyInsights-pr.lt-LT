---
title: "\"Apple\" automatinio įrenginio registracijos Sinchronizavimo klaidos"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448930"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="2e7af-102">"Apple" automatinio įrenginio registracijos Sinchronizavimo klaidos</span><span class="sxs-lookup"><span data-stu-id="2e7af-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="2e7af-103">"Nustatėme, kad turite vieną ar daugiau ad/DEP žetonų, kurie yra klaidos būsenos.</span><span class="sxs-lookup"><span data-stu-id="2e7af-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="2e7af-104">Tol, kol bus išspręsta kiekvieno paveikto atpažinimo ženklo klaidos būsena, funkcija Ada neveiks taip, kaip tikėtasi. ".</span><span class="sxs-lookup"><span data-stu-id="2e7af-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="2e7af-105">Ši klaida gali pasireikšti įvairiais būdais, įskaitant:</span><span class="sxs-lookup"><span data-stu-id="2e7af-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="2e7af-106">Įrenginių negalima sinchronizuoti iš ABM/ASM į Intune</span><span class="sxs-lookup"><span data-stu-id="2e7af-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="2e7af-107">Registracijos profilio priskyrimai gali būti nepavykę</span><span class="sxs-lookup"><span data-stu-id="2e7af-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="2e7af-108">Įrenginiai gali sėkmingai neužbaigti ADE įtraukimo</span><span class="sxs-lookup"><span data-stu-id="2e7af-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="2e7af-109">Patikrinkite, ar sinchronizavimo klaida, pateikta "Intune" konsolėje, dalyje **įrenginiai > registruotis įrenginiai > "Apple" registracija > registracijos programos atpažinimo ženklai**.</span><span class="sxs-lookup"><span data-stu-id="2e7af-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="2e7af-110">Viena dažniausių Sinchronizavimo klaidos priežasčių yra dabartinio atpažinimo ženklo galiojimo laikas.</span><span class="sxs-lookup"><span data-stu-id="2e7af-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="2e7af-111">Daugeliu atvejų paveikto atpažinimo ženklo atnaujinimas padės išspręsti problemą.</span><span class="sxs-lookup"><span data-stu-id="2e7af-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="2e7af-112">Jei vieno arba kelių jūsų žetonų galiojimas baigėsi, peržiūrėkite toliau pateiktus dokumentus, kad galėtumėte juos atnaujinti:</span><span class="sxs-lookup"><span data-stu-id="2e7af-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="2e7af-113">Automatinio įrenginio registracijos atpažinimo ženklo atnaujinimas</span><span class="sxs-lookup"><span data-stu-id="2e7af-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="2e7af-114">Be to, galite matyti toliau pateiktus dokumentus, kad matytumėte galimus kitų klaidų, sukėlusio simbolinės sinchronizavimo triktis, taisymus:</span><span class="sxs-lookup"><span data-stu-id="2e7af-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="2e7af-115">ABM/ASM Sinchronizavimo klaidos, skirtos "iOS"/iPadOS ir "macOS" Automatizuotiems įrenginio registracijos žetonams</span><span class="sxs-lookup"><span data-stu-id="2e7af-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="2e7af-116">ABM/ASM Sinchronizavimo klaidos, skirtos "iOS"/iPadOS ir "macOS" Automatizuotiems įrenginio registracijos žetonams</span><span class="sxs-lookup"><span data-stu-id="2e7af-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
