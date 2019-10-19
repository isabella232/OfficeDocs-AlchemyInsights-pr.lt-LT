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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36505002"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="10755-102">Sąlyginė prieiga su Intune</span><span class="sxs-lookup"><span data-stu-id="10755-102">Conditional Access with Intune</span></span>

<span data-ttu-id="10755-103">Naudojant **sąlyginę prieigą** su Intune reikia 3 žingsniai:</span><span class="sxs-lookup"><span data-stu-id="10755-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="10755-104">Sukurkite **sąlyginę prieigos strategiją** , kuri apibrėžia, kurie ištekliai yra apsaugoti, ir kokias sąlygas reikia atitikti norint pasiekti šiuos išteklius.</span><span class="sxs-lookup"><span data-stu-id="10755-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="10755-105">Pvz., įrenginys turi būti suderinamas prieš pasiekiant įmonės el. paštą.</span><span class="sxs-lookup"><span data-stu-id="10755-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="10755-106">Sukurkite **atitikties strategiją** , kad apibrėžtumėte parametrus, kuriuos reikia įvykdyti, kad įrenginys būtų laikomas atitinkančiu reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="10755-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="10755-107">Pvz., įrenginys turi turėti bent 6 skaitmenų kaištį prieš tai, kai jis laikomas atitinkančiu reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="10755-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="10755-108">Užtikrinti **atitikties politiką** ir **sąlyginės prieigos strategijos** yra skirtos norimos grupės vartotojams.</span><span class="sxs-lookup"><span data-stu-id="10755-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="10755-109">Tam gali reikėti sukurti konkrečias vartotojų grupes "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="10755-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="10755-110">Skaityti daugiau:</span><span class="sxs-lookup"><span data-stu-id="10755-110">Read more:</span></span>
  
- [<span data-ttu-id="10755-111">Sąlyginė prieiga geriausia praktika</span><span class="sxs-lookup"><span data-stu-id="10755-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="10755-112">Darbo su sąlygine prieiga Pradžia</span><span class="sxs-lookup"><span data-stu-id="10755-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

