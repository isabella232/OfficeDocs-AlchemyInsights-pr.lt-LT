---
title: Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826099"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="a935b-102">Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos</span><span class="sxs-lookup"><span data-stu-id="a935b-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="a935b-103">Bandant nustatyti arba peržiūrėti AllowSelfServicePurchase strategiją, rodomas toks klaidos pranešimas:</span><span class="sxs-lookup"><span data-stu-id="a935b-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="a935b-104">*HandleError : nepavyko gauti produkto strategijos su PolicyId 'AllowSelfServicePurchase', ErrorMessage – pagrindinis ryšys buvo uždarytas: siunčiant įvyko netikėta klaida.*</span><span class="sxs-lookup"><span data-stu-id="a935b-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="a935b-105">Taip gali būti dėl senesnės transportavimo lygmens saugos (TLS) versijos.</span><span class="sxs-lookup"><span data-stu-id="a935b-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="a935b-106">Norėdami prijungti MSCommerce tarnybą, turite naudoti TLS 1.2 arba didesnę.</span><span class="sxs-lookup"><span data-stu-id="a935b-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="a935b-107">Pabandykite atlikti šiuos veiksmus, kad įgalintumėte / nustatykite TLS protokolą kaip 1.2, patikrinkite ir bandykite dar kartą.</span><span class="sxs-lookup"><span data-stu-id="a935b-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="a935b-108">"PowerShell" komandinėje eilutėje (PS C: įveskite šią komandą, kad \) TLS protokolą nustatytų kaip 1.2 versiją:</span><span class="sxs-lookup"><span data-stu-id="a935b-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="a935b-109">Patikrinkite, ar naudojamas (-i) TLS protokolas (-ai), naudodami šią komandą:</span><span class="sxs-lookup"><span data-stu-id="a935b-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="a935b-110">Iš naujo bandykite komandas Gauti arba Naujinti, jei reikia.</span><span class="sxs-lookup"><span data-stu-id="a935b-110">Retry the Get or Update commands as needed.</span></span>

