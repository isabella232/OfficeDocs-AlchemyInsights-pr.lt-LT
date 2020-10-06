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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366436"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="fe1f3-102">"Exchange" sąlyginės prieigos stebėjimas</span><span class="sxs-lookup"><span data-stu-id="fe1f3-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="fe1f3-103">Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="fe1f3-104">Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="fe1f3-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="fe1f3-105">Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="fe1f3-106">Jei ne, vartotojas turi registruotis įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="fe1f3-107">"Azure" portale eikite į Intune > įrenginio atitiktis.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="fe1f3-108">Dalyje monitorius spustelėkite įrenginio atitiktis.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="fe1f3-109">Peržiūrėkite savo įrenginio atitikties ataskaitą, kad patikrintumėte, ar vartotojo įrenginys pažymėtas kaip suderinamas.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="fe1f3-110">"Azure" portale eikite į Intune > įrenginio atitiktis.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="fe1f3-111">Dalyje tvarkyti spustelėkite strategijos.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-111">Under Manage, click Policies.</span></span> <span data-ttu-id="fe1f3-112">Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="fe1f3-113">Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="fe1f3-114">Vartotojo sąlyginės prieigos priskyrimo redagavimas.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="fe1f3-115">"Azure" portale eikite į " **Intune**"  >  **sąlyginės prieigos**  >  **strategijas**.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="fe1f3-116">Sąraše pasirinkite strategiją.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="fe1f3-117">Spustelėkite vartotojai ir grupės.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-117">Click Users and groups.</span></span>
4. <span data-ttu-id="fe1f3-118">Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į sąrašą įtraukti.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="fe1f3-119">Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į sąrašą neįtraukti.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="fe1f3-120">Naudingi saitai:</span><span class="sxs-lookup"><span data-stu-id="fe1f3-120">Helpful links:</span></span>

[<span data-ttu-id="fe1f3-121">Įrenginio atitikties apžvalga</span><span class="sxs-lookup"><span data-stu-id="fe1f3-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="fe1f3-122">Trikčių diagnostika CA</span><span class="sxs-lookup"><span data-stu-id="fe1f3-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="fe1f3-123">Trikčių šalinimo strategija</span><span class="sxs-lookup"><span data-stu-id="fe1f3-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="fe1f3-124">"Intune" įrenginio atitikties stebėjimas</span><span class="sxs-lookup"><span data-stu-id="fe1f3-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="fe1f3-125">Pastaba: šie veiksmai naudingi tik šalinant "Azure Active Directory" funkcijos sąlyginę prieigą.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="fe1f3-126">Taip pat galima sulaikyti įrenginį, kuris blokuoja prieigą prie "Exchange" strategijos.</span><span class="sxs-lookup"><span data-stu-id="fe1f3-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="fe1f3-127">Daugiau informacijos apie "Exchange" įrenginių valdymą rasite [čia](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="fe1f3-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
