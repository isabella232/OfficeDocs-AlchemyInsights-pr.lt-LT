---
title: Domeno valdiklis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901028"
---
# <a name="domain-controller"></a><span data-ttu-id="71033-102">Domeno valdiklis</span><span class="sxs-lookup"><span data-stu-id="71033-102">Domain controller</span></span>

<span data-ttu-id="71033-103">**Nepavyksta įjungti "AAD" arba diegimo.**</span><span class="sxs-lookup"><span data-stu-id="71033-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="71033-104">Jei norite išspręsti "Azure AD" domenų tarnybos (AAD – DS) problemą, kuri neįgalinta arba nepavyksta įdiegti, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="71033-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="71033-105">Jei naudojate jau esamą virtualiojo tinklo, patikrinkite savo NSG taisykles, kurios blokuoja prievadus, reikalingus sinchronizuoti naudojant "AAD-DS" portale https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="71033-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="71033-106">Patikrinkite, ar jūsų klaidos pranešimas atsakomas šiame trikčių diagnostikos vadove, kuris pasiekiamas  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="71033-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="71033-107">Pabandykite diegti "Azure AD" domenų tarnybas naujame virtualiame tinkle.</span><span class="sxs-lookup"><span data-stu-id="71033-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="71033-108">Vadovaukitės darbo pradžios vadovu, kaip įdiegti "AAD-DS", kurį galima naudoti [mokymo programoje "AZURE AD" domenų paslaugoms kurti](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="71033-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="71033-109">Jei kyla problemų diegiant "Azure AD" domenų tarnybas, peržiūrėkite " [AZURE AD" domenų tarnybų trikčių šalinimas](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , kad būtų išspręstos Dažniausios klaidos, padedančios gauti darbą dar kartą.</span><span class="sxs-lookup"><span data-stu-id="71033-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="71033-110">**Negalima išjungti AAD – DS**</span><span class="sxs-lookup"><span data-stu-id="71033-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="71033-111">AAD – DS negali būti pristabdytas.</span><span class="sxs-lookup"><span data-stu-id="71033-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="71033-112">Jei nebenorite naudoti valdomo domeno, jį reikia naikinti.</span><span class="sxs-lookup"><span data-stu-id="71033-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="71033-113">Jei susidūrėte su problemomis, Norėdami išspręsti dažnai pasitaikančių klaidų ir susijusių trikčių šalinimo veiksmus, kad galėtumėte vėl atlikti veiksmus, skaitykite " [Azure Active Directory" domenų tarnybos trikčių šalinimas](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="71033-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
