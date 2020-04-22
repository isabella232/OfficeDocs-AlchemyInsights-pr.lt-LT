---
title: Sąlyginė prieiga su "Intune"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706029"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="a4169-102">Sąlyginė prieiga su "Intune"</span><span class="sxs-lookup"><span data-stu-id="a4169-102">Conditional Access with Intune</span></span>

<span data-ttu-id="a4169-103">Norint naudoti **sąlyginę prieigą** su "Intune", reikia atlikti 3 veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a4169-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="a4169-104">**Sukurkite sąlyginės prieigos strategiją,** kuri apibrėžia, kokie ištekliai yra saugomi ir kokios sąlygos turi būti įvykdytos norint pasiekti šiuos išteklius.</span><span class="sxs-lookup"><span data-stu-id="a4169-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="a4169-105">Pavyzdžiui, įrenginys turi atitikti reikalavimus prieš prisijungdamas prie įmonės el. pašto.</span><span class="sxs-lookup"><span data-stu-id="a4169-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="a4169-106">Sukurkite **atitikties strategiją,** kad nustatytumėte parametrus, kurių reikia laikyti įvykdytais prieš laikant įrenginiusuderinamus.</span><span class="sxs-lookup"><span data-stu-id="a4169-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="a4169-107">Pavyzdžiui, prieš jį laikant atitinkančiu įtaisu, įrenginys turi turėti bent 6 skaitmenų kaištį.</span><span class="sxs-lookup"><span data-stu-id="a4169-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="a4169-108">Atitikties **politikos** ir **sąlyginės prieigos strategijų** užtikrinimas būtų nukreiptas į norimas vartotojų grupes.</span><span class="sxs-lookup"><span data-stu-id="a4169-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="a4169-109">Tam gali reikėti kurti konkrečias vartotojų grupes "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="a4169-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="a4169-110">Skaityti daugiau:</span><span class="sxs-lookup"><span data-stu-id="a4169-110">Read more:</span></span>
  
- [<span data-ttu-id="a4169-111">Sąlyginės prieigos geriausios praktikos pavyzdžiai</span><span class="sxs-lookup"><span data-stu-id="a4169-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="a4169-112">Darbo su sąlygine prieiga pradžia</span><span class="sxs-lookup"><span data-stu-id="a4169-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

