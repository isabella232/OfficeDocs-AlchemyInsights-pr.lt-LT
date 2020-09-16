---
title: Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735207"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="f75bb-102">Negalima nustatyti arba peržiūrėti AllowSelfServicePurchase strategijos</span><span class="sxs-lookup"><span data-stu-id="f75bb-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="f75bb-103">Kai bandote nustatyti arba peržiūrėti AllowSelfServicePurchase strategiją, gaunate šį klaidos pranešimą:</span><span class="sxs-lookup"><span data-stu-id="f75bb-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="f75bb-104">*HandleError: nepavyko gauti produkto strategijos su strategijos ID "AllowSelfServicePurchase", ErrorMessage – esamas prisijungimas buvo uždarytas: įvyko netikėta klaida siunčiant.*</span><span class="sxs-lookup"><span data-stu-id="f75bb-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="f75bb-105">Taip gali būti dėl senesnės transportavimo lygmens saugos (TLS) versijos.</span><span class="sxs-lookup"><span data-stu-id="f75bb-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="f75bb-106">Norėdami prijungti MSCommerce paslaugą, turite naudoti TLS 1,2 arba daugiau.</span><span class="sxs-lookup"><span data-stu-id="f75bb-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="f75bb-107">Pabandykite atlikti toliau nurodytus veiksmus, kad įgalintumėte/nustatytumėte TLS protokolą iki 1,2, patikrinti ir bandyti dar kartą.</span><span class="sxs-lookup"><span data-stu-id="f75bb-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="f75bb-108">"PowerShell" komandų eilutėje (PS C: \) įvesti šią komandą, kad TLS protokolas būtų nustatytas į 1,2 versiją:</span><span class="sxs-lookup"><span data-stu-id="f75bb-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="f75bb-109">Patikrinkite naudojamą TLS protokolą (-us), naudodami šią komandą:</span><span class="sxs-lookup"><span data-stu-id="f75bb-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="f75bb-110">Jei reikia, iš naujo bandykite gauti arba atnaujinti komandas.</span><span class="sxs-lookup"><span data-stu-id="f75bb-110">Retry the Get or Update commands as needed.</span></span>

