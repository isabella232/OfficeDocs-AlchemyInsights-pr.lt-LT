---
title: Sąlyginės prieigos naudojimas su Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693580"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="7e5d1-102">Sąlyginės prieigos naudojimas su Intune</span><span class="sxs-lookup"><span data-stu-id="7e5d1-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="7e5d1-103">Naudojant sąlyginę prieigą su Intune reikia 3 veiksmų:</span><span class="sxs-lookup"><span data-stu-id="7e5d1-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="7e5d1-104">Sukurkite atitikties strategiją, kad nustatytumėte parametrus, kurie turi būti įvykdyti prieš tai, kai įrenginys laikomas atitinkančiu reikalavimus. Pvz., įrenginyje turi būti bent 6 skaitmenų PIN, kad jis būtų laikomas atitinkančiu reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="7e5d1-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="7e5d1-105">Sukurkite sąlyginės prieigos strategiją, kuri apibrėžia, kokie ištekliai yra saugomi, ir kokiomis sąlygomis reikia pasiekti šiuos išteklius. Pavyzdžiui, įrenginys turi būti suderinamas prieš jungiantis prie įmonės elektroninio pašto.</span><span class="sxs-lookup"><span data-stu-id="7e5d1-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="7e5d1-106">Užtikrinkite, kad atitikties strategijos ir sąlyginės prieigos strategijos būtų nukreiptos į pageidaujamas vartotojų grupes. Tam gali reikėti sukurti tam tikras vartotojų grupes "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="7e5d1-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7e5d1-107">Skaitykite daugiau...</span><span class="sxs-lookup"><span data-stu-id="7e5d1-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
