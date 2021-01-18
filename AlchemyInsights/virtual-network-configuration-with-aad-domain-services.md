---
title: Virtuali konfigūracija su "AAD" domenų tarnybomis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885643"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="71e3a-102">Virtuali konfigūracija su "AAD" domenų tarnybomis</span><span class="sxs-lookup"><span data-stu-id="71e3a-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="71e3a-103">Virtualioji konfigūracija su "AAD" domenų tarnybomis apima šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="71e3a-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="71e3a-104">Domeno sveikatos tikrinimas "Azure" portale https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="71e3a-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="71e3a-105">"NSG" tikrinimo taisyklės, kurios blokuoja prievadus, reikalingus sinchronizuoti "Azure AD" domenų tarnybose portale https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="71e3a-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="71e3a-106">Užtikrinti, kad jūsų virtualus tinklas būtų įdiegtas tame pačiame "Azure" regione kaip jūsų "Azure AD" domenų tarnybos valdomas domenas.</span><span class="sxs-lookup"><span data-stu-id="71e3a-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="71e3a-107">Užtikrinti, kad neturite esamo domeno su tuo pačiu domeno pavadinimu, kurį galima naudoti virtualiame tinkle.</span><span class="sxs-lookup"><span data-stu-id="71e3a-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="71e3a-108">Daugiau informacijos apie dizaino atlygį "Azure" virtualiame tinkle, siekiant palaikyti "AAD" domenų tarnybas, ieškokite [virtualiojo tinklo nagrinėjimo](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="71e3a-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

