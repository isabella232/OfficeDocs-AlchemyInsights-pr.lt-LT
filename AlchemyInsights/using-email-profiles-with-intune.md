---
title: El. pašto profilių naudojimas su "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555251"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="2b3b0-102">El. pašto profilių naudojimas su "Intune"</span><span class="sxs-lookup"><span data-stu-id="2b3b0-102">Using email profiles with Intune</span></span>

<span data-ttu-id="2b3b0-103">Intune gali būti naudojamas sukurti ir įdiegti el. pašto profilius gimtoji (built-in) el. pašto klientas keliose įrenginių platformose.</span><span class="sxs-lookup"><span data-stu-id="2b3b0-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="2b3b0-104">Informacijos apie kai kuriuos apribojimus, susijusius su el. pašto profiliais, įskaitant tai, kaip tvarkomi esami profiliai ir kaip pašalinti el. pašto profilius, rasite [El. pašto parametrų įtraukimas į įrenginius naudojant "Intune".](https://docs.microsoft.com/intune/email-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="2b3b0-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="2b3b0-105">Jei norite gauti daugiau informacijos apie tai, kaip sukurti el. pašto profilius kiekvienai įrenginio platformai, žr.:</span><span class="sxs-lookup"><span data-stu-id="2b3b0-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="2b3b0-106">"Android" įrenginio nustatymai, norint konfigūruoti el. paštą, autentifikavimą ir sinchronizavimą "Intune"</span><span class="sxs-lookup"><span data-stu-id="2b3b0-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="2b3b0-107">"iOS" ir "iPadOS" įrenginių el. pašto parametrų įtraukimas programoje "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="2b3b0-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="2b3b0-108">El. pašto profilio parametrai programoje "Microsoft Intune" įrenginiuose, kuriuose veikia "Windows Phone 8.1"</span><span class="sxs-lookup"><span data-stu-id="2b3b0-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="2b3b0-109">El. pašto profilio parametrai įrenginiams, kuriuose veikia "Windows 10" programoje "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="2b3b0-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="2b3b0-110">**Dažna sinchronizavimo problema**</span><span class="sxs-lookup"><span data-stu-id="2b3b0-110">**Common syncing issue**</span></span>

<span data-ttu-id="2b3b0-111">**"Knox" "Android" el. pašto profilyje neleidžia naudotojams sinchronizuoti kontaktų, kalendoriaus ir užduočių su naudotojo įrenginiais.**</span><span class="sxs-lookup"><span data-stu-id="2b3b0-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="2b3b0-112">"Knox" "Android KNOX" el. pašto profilyje administratoriui suteikiama galimybė nuspręsti, kurie turinio tipai sinchronizuojami su įrenginiu, nustatant kiekvieną įjungtą.</span><span class="sxs-lookup"><span data-stu-id="2b3b0-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="2b3b0-113">Jei kurio nors turinio tipo parametras nustatytas kaip **Nesukonfigūruotas** (numatytasis), tas turinio tipas automatiškai nesinchronizuojamas.</span><span class="sxs-lookup"><span data-stu-id="2b3b0-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="2b3b0-114">Vartotojas gali įgalinti turinio tipą, kurio jis nori tiesiogiai įrenginyje, rankiniu būdu, bet šią konfigūraciją perrašo "Intune" strategijos parametras, o sinchronizavimas sustabdomas to turinio tipui.</span><span class="sxs-lookup"><span data-stu-id="2b3b0-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

