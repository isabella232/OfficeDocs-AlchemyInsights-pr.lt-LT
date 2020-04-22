---
title: Sąlyginės prieigos stebėjimas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713726"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="d26b6-102">Sąlyginės prieigos mainams stebėjimas</span><span class="sxs-lookup"><span data-stu-id="d26b6-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="d26b6-103">Vartotojai, kuriems taikoma sąlyginė prieiga, gaus pranešimo el. laišką, jei neatitinka jūsų organizacijos prieigos reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="d26b6-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="d26b6-104">Norėdami išspręsti, rekomenduojame vieną ar daugiau iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="d26b6-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="d26b6-105">Jei manoma, kad įrenginys bus įtrauktas, patarkite vartotojui eiti į įmonės portalo programėlę ir patikrinti, ar jis rodomas įmonės portale.</span><span class="sxs-lookup"><span data-stu-id="d26b6-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="d26b6-106">Jei ne, vartotojas turėtų užregistruoti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="d26b6-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="d26b6-107">Azure portale eikite į **Intune \> įrenginio atitiktis**.</span><span class="sxs-lookup"><span data-stu-id="d26b6-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="d26b6-108">Dalyje **Monitorius** spustelėkite **Įrenginio atitiktis**.</span><span class="sxs-lookup"><span data-stu-id="d26b6-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="d26b6-109">Peržiūrėkite įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas.</span><span class="sxs-lookup"><span data-stu-id="d26b6-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="d26b6-110">Azure portale eikite į **Intune \> įrenginio atitiktis**.</span><span class="sxs-lookup"><span data-stu-id="d26b6-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="d26b6-111">Dalyje **Tvarkyti**spustelėkite **Strategijos**.</span><span class="sxs-lookup"><span data-stu-id="d26b6-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="d26b6-112">Atitikties strategijų sąraše patikrinkite, ar jūsų vartotojo įrenginiui priskirtas profilis.</span><span class="sxs-lookup"><span data-stu-id="d26b6-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="d26b6-113">Jei profilis nepriskirtas, "Intune" negalės patvirtinti įrenginio atitikties būsenos.</span><span class="sxs-lookup"><span data-stu-id="d26b6-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="d26b6-114">Redaguokite vartotojo sąlyginės prieigos priskyrimą.</span><span class="sxs-lookup"><span data-stu-id="d26b6-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="d26b6-115">Azure portale eikite į **Intune \> sąlyginės prieigos \> strategijos**</span><span class="sxs-lookup"><span data-stu-id="d26b6-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="d26b6-116">Pasirinkite strategiją iš sąrašo</span><span class="sxs-lookup"><span data-stu-id="d26b6-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="d26b6-117">Spustelėkite **Vartotojai ir grupės**</span><span class="sxs-lookup"><span data-stu-id="d26b6-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="d26b6-118">Norėdami taikyti pagal tam tikrą strategiją kam nors, įtraukite ją į sąrašą **Įtraukti.**</span><span class="sxs-lookup"><span data-stu-id="d26b6-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="d26b6-119">Norėdami užtikrinti, kad asmuo nebūtų įtrauktas į strategiją, įtraukite jį į **sąrašą Neįtraukti.**</span><span class="sxs-lookup"><span data-stu-id="d26b6-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="d26b6-120">Skaityti daugiau: [Kaip stebėti sąlyginės prieigos įrenginius](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="d26b6-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

