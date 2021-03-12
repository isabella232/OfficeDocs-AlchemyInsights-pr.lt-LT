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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708682"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="06abb-102">"Exchange" sąlyginės prieigos stebėjimas</span><span class="sxs-lookup"><span data-stu-id="06abb-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="06abb-103">Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="06abb-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="06abb-104">Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="06abb-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="06abb-105">Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale.</span><span class="sxs-lookup"><span data-stu-id="06abb-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="06abb-106">Jei ne, vartotojas turi registruotis įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="06abb-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="06abb-107">"Azure" portale eikite į Intune > įrenginio atitiktis.</span><span class="sxs-lookup"><span data-stu-id="06abb-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="06abb-108">Dalyje monitorius spustelėkite įrenginio atitiktis.</span><span class="sxs-lookup"><span data-stu-id="06abb-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="06abb-109">Peržiūrėkite savo įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas.</span><span class="sxs-lookup"><span data-stu-id="06abb-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="06abb-110">"Azure" portale eikite į Intune > įrenginio atitiktis.</span><span class="sxs-lookup"><span data-stu-id="06abb-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="06abb-111">Dalyje tvarkyti spustelėkite strategijos.</span><span class="sxs-lookup"><span data-stu-id="06abb-111">Under Manage, click Policies.</span></span> <span data-ttu-id="06abb-112">Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="06abb-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="06abb-113">Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos.</span><span class="sxs-lookup"><span data-stu-id="06abb-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="06abb-114">Vartotojo sąlyginės prieigos priskyrimo redagavimas.</span><span class="sxs-lookup"><span data-stu-id="06abb-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="06abb-115">"Azure" portale eikite į " **Intune**"  >  **sąlyginės prieigos**  >  **strategijas**.</span><span class="sxs-lookup"><span data-stu-id="06abb-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="06abb-116">Sąraše pasirinkite strategiją.</span><span class="sxs-lookup"><span data-stu-id="06abb-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="06abb-117">Spustelėkite vartotojai ir grupės.</span><span class="sxs-lookup"><span data-stu-id="06abb-117">Click Users and groups.</span></span>
4. <span data-ttu-id="06abb-118">Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į sąrašą įtraukti.</span><span class="sxs-lookup"><span data-stu-id="06abb-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="06abb-119">Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į sąrašą neįtraukti.</span><span class="sxs-lookup"><span data-stu-id="06abb-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="06abb-120">Naudingi saitai:</span><span class="sxs-lookup"><span data-stu-id="06abb-120">Helpful links:</span></span>

[<span data-ttu-id="06abb-121">Įrenginio atitikties apžvalga</span><span class="sxs-lookup"><span data-stu-id="06abb-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="06abb-122">Trikčių diagnostika CA</span><span class="sxs-lookup"><span data-stu-id="06abb-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="06abb-123">Trikčių šalinimo strategija</span><span class="sxs-lookup"><span data-stu-id="06abb-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="06abb-124">"Intune" įrenginio atitikties stebėjimas</span><span class="sxs-lookup"><span data-stu-id="06abb-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="06abb-125">Pastaba: šie veiksmai naudingi tik šalinant "Azure Active Directory" funkcijos sąlyginę prieigą.</span><span class="sxs-lookup"><span data-stu-id="06abb-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="06abb-126">Taip pat galima sulaikyti įrenginį, kuris blokuoja prieigą prie "Exchange" strategijos.</span><span class="sxs-lookup"><span data-stu-id="06abb-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="06abb-127">Daugiau informacijos apie "Exchange" įrenginių valdymą galima rasti [čia] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="06abb-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
