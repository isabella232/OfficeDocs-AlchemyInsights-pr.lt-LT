---
title: "\"Apple\" automatinio įrenginio registracijos Sinchronizavimo klaidos"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714830"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="81d5c-102">"Apple" automatinio įrenginio registracijos Sinchronizavimo klaidos</span><span class="sxs-lookup"><span data-stu-id="81d5c-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="81d5c-103">"Nustatėme, kad turite vieną ar daugiau ad/DEP žetonų, kurie yra klaidos būsenos.</span><span class="sxs-lookup"><span data-stu-id="81d5c-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="81d5c-104">Kol klaidos būsena bus išspręsta kiekvienam paveiktam žetonu, "Ada" funkcijos neveiks tame pačiame ".</span><span class="sxs-lookup"><span data-stu-id="81d5c-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="81d5c-105">Ši klaida gali pasireikšti įvairiais būdais, įskaitant:</span><span class="sxs-lookup"><span data-stu-id="81d5c-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="81d5c-106">Įrenginių negalima sinchronizuoti iš ABM/ASM į Intune</span><span class="sxs-lookup"><span data-stu-id="81d5c-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="81d5c-107">Registracijos profilio priskyrimai gali būti nepavykę</span><span class="sxs-lookup"><span data-stu-id="81d5c-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="81d5c-108">Įrenginiai gali sėkmingai neužbaigti ADE įtraukimo</span><span class="sxs-lookup"><span data-stu-id="81d5c-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="81d5c-109">Patikrinkite, ar sinchronizavimo klaida, pateikta "Intune" konsolėje, dalyje **įrenginiai > registruotis įrenginiai > "Apple" registracija > registracijos programos atpažinimo ženklai** ir peržiūrėkite toliau pateiktus dokumentus, kad pamatytumėte galimą išvalimą:</span><span class="sxs-lookup"><span data-stu-id="81d5c-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="81d5c-110">ABM/ASM Sinchronizavimo klaidos, skirtos "iOS"/iPadOS ir "macOS" Automatizuotiems įrenginio registracijos žetonams</span><span class="sxs-lookup"><span data-stu-id="81d5c-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
