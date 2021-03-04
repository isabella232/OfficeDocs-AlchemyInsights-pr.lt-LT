---
title: "\"Intune\" sąlyginės prieigos stebėjimas"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427923"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="233b8-102">"Intune" sąlyginės prieigos stebėjimas</span><span class="sxs-lookup"><span data-stu-id="233b8-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="233b8-103">Vartotojai, kurie orientuoti naudojant sąlyginę prieigą, gaus pranešimą elektroniniu paštu, jei jie neatitinka jūsų organizacijos prieigos reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="233b8-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="233b8-104">Norėdami išspręsti problemą, rekomenduojame vieną ar kelis iš šių sprendimų:</span><span class="sxs-lookup"><span data-stu-id="233b8-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="233b8-105">Jei manoma, kad įrenginys bus užregistruotas, patarkite vartotojui eiti į įmonės portalo programą ir patikrinkite, ar ji rodoma įmonės portale.</span><span class="sxs-lookup"><span data-stu-id="233b8-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="233b8-106">Jei ne, vartotojas turi užregistruoti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="233b8-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="233b8-107">"Azure" portale eikite į " **Intune**"  >  **įrenginio atitiktį**.</span><span class="sxs-lookup"><span data-stu-id="233b8-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="233b8-108">Norėdami peržiūrėti įrenginio atitikties ataskaitą, kad įsitikintumėte, jog vartotojo įrenginys pažymėtas kaip suderinamas, dalyje **monitorius** spustelėkite **įrenginio atitiktis**.</span><span class="sxs-lookup"><span data-stu-id="233b8-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="233b8-109">"Azure" portale eikite į " **Intune**"  >  **įrenginio atitiktį**.</span><span class="sxs-lookup"><span data-stu-id="233b8-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="233b8-110">Dalyje **tvarkyti** spustelėkite **strategijos**.</span><span class="sxs-lookup"><span data-stu-id="233b8-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="233b8-111">Atitikties strategijų sąraše patikrinkite, ar profilis priskirtas jūsų vartotojo įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="233b8-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="233b8-112">Jei nepriskirtas joks profilis, tada Intune negalės patvirtinti įrenginio atitikties būsenos.</span><span class="sxs-lookup"><span data-stu-id="233b8-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="233b8-113">Vartotojo sąlyginės prieigos priskyrimo redagavimas.</span><span class="sxs-lookup"><span data-stu-id="233b8-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="233b8-114">"Azure" portale eikite į **Intune**  >  **sąlyginės prieigos**  >  **strategijas**, iš sąrašo pasirinkite strategiją ir spustelėkite **vartotojai ir grupės**.</span><span class="sxs-lookup"><span data-stu-id="233b8-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="233b8-115">Norėdami nukreipti tam tikrą strategiją į ką nors, įtraukite jas į **sąrašą įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="233b8-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="233b8-116">Norėdami užtikrinti, kad asmuo būtų praleistas strategijoje, įtraukite juos į **sąrašą neįtraukti**.</span><span class="sxs-lookup"><span data-stu-id="233b8-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="233b8-117">**Naudingi saitai:**</span><span class="sxs-lookup"><span data-stu-id="233b8-117">**Helpful links:**</span></span>

- [<span data-ttu-id="233b8-118">Įrenginio atitikties apžvalga</span><span class="sxs-lookup"><span data-stu-id="233b8-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="233b8-119">Trikčių diagnostika CA</span><span class="sxs-lookup"><span data-stu-id="233b8-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="233b8-120">Trikčių šalinimo strategija</span><span class="sxs-lookup"><span data-stu-id="233b8-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="233b8-121">"Intune" įrenginio atitikties stebėjimas</span><span class="sxs-lookup"><span data-stu-id="233b8-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="233b8-122">Šie veiksmai yra naudingi šalinant "Azure Active Directory" funkcijos sąlyginę prieigą.</span><span class="sxs-lookup"><span data-stu-id="233b8-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="233b8-123">Taip pat galima sulaikyti įrenginį, kuris blokuoja prieigą prie "Exchange" strategijos.</span><span class="sxs-lookup"><span data-stu-id="233b8-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="233b8-124">Daugiau informacijos apie "Exchange" įrenginių valdymą rasite [**čia**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="233b8-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
