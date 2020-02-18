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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091734"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="4d02c-102">Neįmanoma nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos</span><span class="sxs-lookup"><span data-stu-id="4d02c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="4d02c-103">Bandant nustatyti arba peržiūrėti AllowSelfServicePurchase strategija, galite gauti tokį klaidos pranešimą:</span><span class="sxs-lookup"><span data-stu-id="4d02c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="4d02c-104">*HandleError: nepavyko gauti produkto politikos su PolicyId "AllowSelfServicePurchase", ErrorMessage-pagrindinis ryšys buvo uždarytas: siuntimo metu įvyko netikėta klaida.*</span><span class="sxs-lookup"><span data-stu-id="4d02c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="4d02c-105">Taip gali būti dėl senesnės versijos transportavimo lygmens saugos (TLS).</span><span class="sxs-lookup"><span data-stu-id="4d02c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="4d02c-106">Norėdami prisijungti prie MSCommerce paslaugos, turite naudoti TLS 1,2 arba didesnis.</span><span class="sxs-lookup"><span data-stu-id="4d02c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="4d02c-107">Pabandykite šiuos veiksmus, Norėdami įjungti/nustatyti TLS protokolo 1,2, patikrinti, ir bandykite dar kartą.</span><span class="sxs-lookup"><span data-stu-id="4d02c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="4d02c-108">"PowerShell" komandinėje eilutėje (PS C\) : įveskite šią komandą, kad TLS protokolo versija 1,2:</span><span class="sxs-lookup"><span data-stu-id="4d02c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="4d02c-109">\[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="4d02c-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="4d02c-110">Patikrinkite, ar TLS protokolo (-ų) naudojimo, su šia komanda:</span><span class="sxs-lookup"><span data-stu-id="4d02c-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="4d02c-111">\[Net. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="4d02c-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="4d02c-112">Bandykite kartoti komandas gauti arba naujinti, jei reikia.</span><span class="sxs-lookup"><span data-stu-id="4d02c-112">Retry the Get or Update commands as needed.</span></span>

