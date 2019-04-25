---
title: Stebėsenos sąlyginės prieigos
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418477"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="28db9-102">Stebėsenos sąlyginės prieigos</span><span class="sxs-lookup"><span data-stu-id="28db9-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="28db9-103">Vartotojams skirta su sąlygine prieiga gausite pranešimas el. paštu, jei jie neatitinka jūsų organizacijos suteikiant prieigą keliami reikalavimai.</span><span class="sxs-lookup"><span data-stu-id="28db9-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="28db9-104">Norėdami išspręsti, rekomenduojame vieną ar kelis iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="28db9-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="28db9-105">Jei prietaisas yra preziumuojamas, gautų, patarti vartotojui eiti į programėlę įmonės portalą ir patikrinkite, ar rodomas įmonės portale.</span><span class="sxs-lookup"><span data-stu-id="28db9-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="28db9-106">Jei ne, vartotojas turėtų registruotis įrenginį.</span><span class="sxs-lookup"><span data-stu-id="28db9-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="28db9-107">Azure portale rasite apsilankę **Intune \> prietaiso atitikties**.</span><span class="sxs-lookup"><span data-stu-id="28db9-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="28db9-108">Po **monitoriumi** spustelėkite **įrenginio atitiktį**.</span><span class="sxs-lookup"><span data-stu-id="28db9-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="28db9-109">Rodyti jūsų prietaiso atitikties ataskaitą, kad patikrinti, kad vartotojo įrenginys pažymimas kaip suderinamas.</span><span class="sxs-lookup"><span data-stu-id="28db9-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="28db9-110">Azure portale rasite apsilankę **Intune \> prietaiso atitikties**.</span><span class="sxs-lookup"><span data-stu-id="28db9-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="28db9-111">Dalyje **tvarkyti**spustelėkite **strategijos**.</span><span class="sxs-lookup"><span data-stu-id="28db9-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="28db9-112">Atitikties strategijos sąraše, patikrinkite, kad profilis yra priskirtas jūsų vartotojo įrenginio.</span><span class="sxs-lookup"><span data-stu-id="28db9-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="28db9-113">Jei nėra Vartotojo profilis yra priskirtas, tada Intune nebus galima patvirtinti įrenginio atitikties būklę.</span><span class="sxs-lookup"><span data-stu-id="28db9-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="28db9-114">Redaguoti vartotojo sąlyginės prieigos priskyrimo.</span><span class="sxs-lookup"><span data-stu-id="28db9-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="28db9-115">Azure portale rasite apsilankę **Intune \> sąlyginės prieigos \> politika**</span><span class="sxs-lookup"><span data-stu-id="28db9-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="28db9-116">Iš sąrašo pasirinkite politiką</span><span class="sxs-lookup"><span data-stu-id="28db9-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="28db9-117">Spustelėkite **vartotojai ir grupės**</span><span class="sxs-lookup"><span data-stu-id="28db9-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="28db9-118">Nukreipti tam tikrą politiką kažkas, įtraukti juos į sąrašus **įtraukti** .</span><span class="sxs-lookup"><span data-stu-id="28db9-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="28db9-119">Siekiant užtikrinti, kad asmuo yra praleista politiką, įtraukti juos į sąrašą **neįtraukti** .</span><span class="sxs-lookup"><span data-stu-id="28db9-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="28db9-120">Skaityti daugiau: [kaip stebėti sąlyginės prieigos priemonės](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="28db9-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

