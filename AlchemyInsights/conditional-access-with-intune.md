---
title: Sąlyginė prieiga su Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935952"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="bc1d6-102">Sąlyginė prieiga su Intune</span><span class="sxs-lookup"><span data-stu-id="bc1d6-102">Conditional Access with Intune</span></span>

<span data-ttu-id="bc1d6-103">**Sąlyginė prieiga** naudojant Intune reikia 3 žingsniai:</span><span class="sxs-lookup"><span data-stu-id="bc1d6-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="bc1d6-p101">Sukurti **Sąlyginis prieigos strategijos** , kuris nustato, kokie ištekliai yra apsaugotas, o kas sąlygos turi atitikti prieiti prie šių išteklių. Pavyzdžiui, įrenginys turi būti suderinamas prieš bandant prieiti prie įmonės el. pašto.</span><span class="sxs-lookup"><span data-stu-id="bc1d6-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="bc1d6-p102">Sukurti **Atitikimo politikos** nustatyti parametrus, kurie turi būti įvykdyti prieš įrenginys yra suderinamas. Pavyzdžiui, įtaisas turi būti mažiausiai 6 skaitmenų pin, kol ji yra laikoma suderinama.</span><span class="sxs-lookup"><span data-stu-id="bc1d6-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="bc1d6-p103">Užtikrinti **Atitikties strategijas** ir **Sąlyginis prieigos strategijos** orientuodamiesi į norimą vartotojų grupių. Gali tekti sukurti Azure Active Directory konkrečių vartotojų grupių.</span><span class="sxs-lookup"><span data-stu-id="bc1d6-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="bc1d6-110">Skaityti daugiau:</span><span class="sxs-lookup"><span data-stu-id="bc1d6-110">Read more:</span></span>
  
- [<span data-ttu-id="bc1d6-111">Sąlyginės prieigos geriausios praktikos</span><span class="sxs-lookup"><span data-stu-id="bc1d6-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="bc1d6-112">Darbo pradžia su sąlygine prieiga</span><span class="sxs-lookup"><span data-stu-id="bc1d6-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

