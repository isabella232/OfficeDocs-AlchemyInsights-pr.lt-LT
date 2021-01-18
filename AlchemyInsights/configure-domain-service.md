---
title: Domeno paslaugos konfigūravimas
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885694"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="ead0d-102">Nepavyksta įjungti "AAD" arba diegimo.</span><span class="sxs-lookup"><span data-stu-id="ead0d-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="ead0d-103">Jei norite išspręsti "Azure AD" domenų tarnybos (AAD – DS) problemą, kuri neįgalinta arba nepavyksta įdiegti, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="ead0d-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="ead0d-104">Jei naudojate jau esamą virtualiojo tinklo, patikrinkite savo NSG taisykles, kurios blokuoja prievadus, reikalingus sinchronizuoti naudojant "AAD-DS" portale https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="ead0d-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="ead0d-105">Patikrinkite, ar jūsų klaidos pranešimas atsakomas šiame trikčių diagnostikos vadove, kuris pasiekiamas  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="ead0d-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="ead0d-106">Pabandykite diegti "Azure AD" domenų tarnybas naujame virtualiame tinkle.</span><span class="sxs-lookup"><span data-stu-id="ead0d-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="ead0d-107">Vadovaukitės darbo pradžios vadovu, kaip įdiegti "AAD-DS": [kurti ir KONFIGŪRUOTI AAD domenų tarnybas](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="ead0d-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="ead0d-108">Jei kyla problemų diegiant "Azure AD" domenų tarnybas, peržiūrėkite " [AZURE AD" domenų tarnybų trikčių šalinimas](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kad būtų išspręstos Dažniausios klaidos, padedančios gauti darbą dar kartą.</span><span class="sxs-lookup"><span data-stu-id="ead0d-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="ead0d-109">**Negalima išjungti AAD – DS**</span><span class="sxs-lookup"><span data-stu-id="ead0d-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="ead0d-110">AAD – DS negali būti pristabdytas.</span><span class="sxs-lookup"><span data-stu-id="ead0d-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="ead0d-111">Jei nebenorite naudoti valdomo domeno, jį reikia naikinti.</span><span class="sxs-lookup"><span data-stu-id="ead0d-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="ead0d-112">Norėdami panaikinti valdomą domeną, žiūrėkite [Naikinti AAD domenų tarnybą](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="ead0d-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



