---
title: "\"Microsoft Edge\" nustatymas kaip numatytosios naršyklės \"macOS\" įrenginyje"
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
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491808"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="32211-102">"Microsoft Edge" nustatymas kaip numatytosios naršyklės "macOS" įrenginyje</span><span class="sxs-lookup"><span data-stu-id="32211-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="32211-103">Norėdami nustatyti "Microsoft Edge" kaip numatytąją naršyklę, naudokite vieną iš šių dviejų būdų:</span><span class="sxs-lookup"><span data-stu-id="32211-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="32211-104">1 būdas: "Flash" įrenginį su "macOS" vaizdu, kuriame "Microsoft Edge" jau nustatyta kaip numatytoji naršyklė.</span><span class="sxs-lookup"><span data-stu-id="32211-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="32211-105">2 būdas: Nustatykite Strategiją DefaultBrowserSettingEnabled, kad vartotojas paragintų nustatyti "Microsoft Edge" kaip numatytąją naršyklę.</span><span class="sxs-lookup"><span data-stu-id="32211-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="32211-106">Bet kuris būdas leidžia vartotojui pakeisti numatytąją naršyklę.</span><span class="sxs-lookup"><span data-stu-id="32211-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="32211-107">Dėl šios priežasties rekomenduojame įdiegti strategiją DefaultBrowserSettingEnabled, net jei naudojote 1 metodą.</span><span class="sxs-lookup"><span data-stu-id="32211-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="32211-108">Jei įdiegus strategiją vartotojas pakeičia numatytąją naršyklę, strategija paragina vartotoją nustatyti numatytąją naršyklę atgal į "Microsoft Edge".</span><span class="sxs-lookup"><span data-stu-id="32211-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
