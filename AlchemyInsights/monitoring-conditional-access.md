---
title: Sąlyginės prieigos stebėjimas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702911"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="2e03e-102">"Exchange" sąlyginės prieigos stebėjimas</span><span class="sxs-lookup"><span data-stu-id="2e03e-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="2e03e-103">Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="2e03e-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2e03e-104">Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="2e03e-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="2e03e-105">Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale.</span><span class="sxs-lookup"><span data-stu-id="2e03e-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2e03e-106">Jei ne, vartotojas turi registruotis įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="2e03e-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="2e03e-107">"Azure" portale eikite į " **Intune" \> įrenginio atitiktį**.</span><span class="sxs-lookup"><span data-stu-id="2e03e-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2e03e-108">Dalyje **monitorius** spustelėkite **įrenginio atitiktis**.</span><span class="sxs-lookup"><span data-stu-id="2e03e-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="2e03e-109">Peržiūrėkite savo įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas.</span><span class="sxs-lookup"><span data-stu-id="2e03e-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="2e03e-110">"Azure" portale eikite į " **Intune" \> įrenginio atitiktį**.</span><span class="sxs-lookup"><span data-stu-id="2e03e-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="2e03e-111">Dalyje **tvarkyti**spustelėkite **strategijos**.</span><span class="sxs-lookup"><span data-stu-id="2e03e-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="2e03e-112">Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="2e03e-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2e03e-113">Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos.</span><span class="sxs-lookup"><span data-stu-id="2e03e-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="2e03e-114">Vartotojo sąlyginės prieigos priskyrimo redagavimas.</span><span class="sxs-lookup"><span data-stu-id="2e03e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="2e03e-115">"Azure" portale eikite į " **Intune" \> sąlyginės prieigos \> strategijas**</span><span class="sxs-lookup"><span data-stu-id="2e03e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="2e03e-116">Sąraše pasirinkite strategiją</span><span class="sxs-lookup"><span data-stu-id="2e03e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="2e03e-117">Spustelėkite **vartotojai ir grupės**</span><span class="sxs-lookup"><span data-stu-id="2e03e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="2e03e-118">Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į sąrašą **įtraukti** .</span><span class="sxs-lookup"><span data-stu-id="2e03e-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="2e03e-119">Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į sąrašą **neįtraukti** .</span><span class="sxs-lookup"><span data-stu-id="2e03e-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="2e03e-120">Skaitykite daugiau: [kaip stebėti sąlyginės prieigos įrenginius](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="2e03e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

