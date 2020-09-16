---
title: El. pašto profilių naudojimas su "Intune"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653296"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="bb653-102">El. pašto profilių naudojimas su "Intune"</span><span class="sxs-lookup"><span data-stu-id="bb653-102">Using email profiles with Intune</span></span>

<span data-ttu-id="bb653-103">Intune gali būti naudojama kuriant ir diegiant "Native" (įtaisytąjį) elektroninio pašto klientą keliuose įrenginių platformose.</span><span class="sxs-lookup"><span data-stu-id="bb653-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="bb653-104">Informacijos apie kai kuriuos apribojimus, susijusius su pašto profiliais, įskaitant tai, kaip tvarkomi esami profiliai ir kaip pašalinti el. pašto profilius, rasite skyriuje [įtraukti el. pašto parametrus į įrenginius](https://docs.microsoft.com/intune/email-settings-configure), kuriuose naudojamas "Intune".</span><span class="sxs-lookup"><span data-stu-id="bb653-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="bb653-105">Daugiau informacijos apie tai, kaip kurti el. pašto profilius kiekvienai įrenginių platformai, ieškokite:</span><span class="sxs-lookup"><span data-stu-id="bb653-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="bb653-106">"Android" įrenginio parametrai, kad sukonfigūruotumėte elektroninio pašto, autentifikavimo ir sinchronizavimo "Intune"</span><span class="sxs-lookup"><span data-stu-id="bb653-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="bb653-107">"Microsoft Intune" "iOS" ir "iPadOS" įrenginių el. pašto parametrų įtraukimas</span><span class="sxs-lookup"><span data-stu-id="bb653-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="bb653-108">"Microsoft Intune" el. pašto profilio parametrai įrenginiams, kuriuose veikia "Windows Phone" 8,1</span><span class="sxs-lookup"><span data-stu-id="bb653-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="bb653-109">"Microsoft Intune" įrenginių, kuriuose veikia "Windows 10", el. pašto profilio parametrai</span><span class="sxs-lookup"><span data-stu-id="bb653-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="bb653-110">**Įprastas sinchronizavimo klausimas**</span><span class="sxs-lookup"><span data-stu-id="bb653-110">**Common syncing issue**</span></span>

<span data-ttu-id="bb653-111">**KNOX, esanti "Android" el. pašto profilyje, apsaugo vartotojų kontaktus, kalendorių ir užduotis, kad nebūtų sinchronizuojama su vartotojų įrenginiais.**</span><span class="sxs-lookup"><span data-stu-id="bb653-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="bb653-112">KNOX "Android KNOX" elektroninio pašto profilyje suteikia administratoriui galimybę nuspręsti, kurie turinio tipai yra sinchronizuojami su įrenginiu, nustatydami kiekvieną įgalintą.</span><span class="sxs-lookup"><span data-stu-id="bb653-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="bb653-113">Jei bet kurio turinio tipo parametras nustatytas kaip **nesukonfigūruotas** (numatytasis parametras), turinio tipas nesinchronizuojamas automatiškai.</span><span class="sxs-lookup"><span data-stu-id="bb653-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="bb653-114">Vartotojas gali įgalinti turinio tipą, kurį jie nori naudoti tiesiogiai įrenginyje, tačiau ši konfigūracija perrašoma iš "Intune" strategijos parametro ir šio turinio tipo sinchronizavimo sustoja.</span><span class="sxs-lookup"><span data-stu-id="bb653-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

