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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505002"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="4cbc2-102">Sąlyginė prieiga su Intune</span><span class="sxs-lookup"><span data-stu-id="4cbc2-102">Conditional Access with Intune</span></span>

<span data-ttu-id="4cbc2-103">**Sąlyginė prieiga** naudojant Intune reikia 3 žingsniai:</span><span class="sxs-lookup"><span data-stu-id="4cbc2-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="4cbc2-104">Sukurti **Sąlyginis prieigos strategijos** , kuris nustato, kokie ištekliai yra apsaugotas, o kas sąlygos turi atitikti prieiti prie šių išteklių.</span><span class="sxs-lookup"><span data-stu-id="4cbc2-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="4cbc2-105">Pavyzdžiui, įrenginys turi būti suderinamas prieš bandant prieiti prie įmonės el. pašto.</span><span class="sxs-lookup"><span data-stu-id="4cbc2-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="4cbc2-106">Sukurti **Atitikimo politikos** nustatyti parametrus, kurie turi būti įvykdyti prieš įrenginys yra suderinamas.</span><span class="sxs-lookup"><span data-stu-id="4cbc2-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="4cbc2-107">Pavyzdžiui, įtaisas turi būti mažiausiai 6 skaitmenų pin, kol ji yra laikoma suderinama.</span><span class="sxs-lookup"><span data-stu-id="4cbc2-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="4cbc2-108">Užtikrinti **Atitikties strategijas** ir **Sąlyginis prieigos strategijos** orientuodamiesi į norimą vartotojų grupių.</span><span class="sxs-lookup"><span data-stu-id="4cbc2-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="4cbc2-109">Gali tekti sukurti Azure Active Directory konkrečių vartotojų grupių.</span><span class="sxs-lookup"><span data-stu-id="4cbc2-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="4cbc2-110">Skaityti daugiau:</span><span class="sxs-lookup"><span data-stu-id="4cbc2-110">Read more:</span></span>
  
- [<span data-ttu-id="4cbc2-111">Sąlyginės prieigos geriausios praktikos</span><span class="sxs-lookup"><span data-stu-id="4cbc2-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="4cbc2-112">Darbo pradžia su sąlygine prieiga</span><span class="sxs-lookup"><span data-stu-id="4cbc2-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

