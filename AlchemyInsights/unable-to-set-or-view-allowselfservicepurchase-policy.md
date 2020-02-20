---
title: Neįmanoma nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158569"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="17187-102">Neįmanoma nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos</span><span class="sxs-lookup"><span data-stu-id="17187-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="17187-103">Bandant nustatyti arba peržiūrėti AllowSelfServicePurchase strategija, galite gauti tokį klaidos pranešimą:</span><span class="sxs-lookup"><span data-stu-id="17187-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="17187-104">*HandleError: nepavyko gauti produkto politikos su PolicyId "AllowSelfServicePurchase", ErrorMessage-pagrindinis ryšys buvo uždarytas: siuntimo metu įvyko netikėta klaida.*</span><span class="sxs-lookup"><span data-stu-id="17187-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="17187-105">Taip gali būti dėl senesnės versijos transportavimo lygmens saugos (TLS).</span><span class="sxs-lookup"><span data-stu-id="17187-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="17187-106">Norėdami prisijungti prie MSCommerce paslaugos, turite naudoti TLS 1,2 arba didesnis.</span><span class="sxs-lookup"><span data-stu-id="17187-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="17187-107">Pabandykite šiuos veiksmus, Norėdami įjungti/nustatyti TLS protokolo 1,2, patikrinti, ir bandykite dar kartą.</span><span class="sxs-lookup"><span data-stu-id="17187-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="17187-108">"PowerShell" komandinėje eilutėje (PS C\) : įveskite šią komandą, kad TLS protokolo versija 1,2:</span><span class="sxs-lookup"><span data-stu-id="17187-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="17187-109">Patikrinkite, ar TLS protokolo (-ų) naudojimo, su šia komanda:</span><span class="sxs-lookup"><span data-stu-id="17187-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="17187-110">Bandykite kartoti komandas gauti arba naujinti, jei reikia.</span><span class="sxs-lookup"><span data-stu-id="17187-110">Retry the Get or Update commands as needed.</span></span>

