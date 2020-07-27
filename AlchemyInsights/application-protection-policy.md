---
title: Taikomųjų programų apsaugos politika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423967"
---
# <a name="application-protection-policy"></a><span data-ttu-id="dfb29-102">Taikomųjų programų apsaugos politika</span><span class="sxs-lookup"><span data-stu-id="dfb29-102">Application protection policy</span></span>

<span data-ttu-id="dfb29-103">Jei pirmą kartą naudojate programos apsaugos strategiją (APP), peržiūrėkite [programėlių apsaugos strategijų apžvalgą](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="dfb29-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="dfb29-104">Norėdami pradėti naudoti APP, [sužinokite, kaip kurti ir priskirti programėlių apsaugos strategijas](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="dfb29-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="dfb29-105">Taikomųjų programų apsaugos strategijos reikalavimai:</span><span class="sxs-lookup"><span data-stu-id="dfb29-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="dfb29-106">Vartotojas turi "Intune" arba EMS licenciją.</span><span class="sxs-lookup"><span data-stu-id="dfb29-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="dfb29-107">Vartotojas priklauso grupei, kuriai taikomos taikomųjų programų apsaugos strategijos.</span><span class="sxs-lookup"><span data-stu-id="dfb29-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="dfb29-108">Tik vienas įmonės naudotojas įrenginyje yra prisijungęs prie apsaugotų programų.</span><span class="sxs-lookup"><span data-stu-id="dfb29-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="dfb29-109">Programa įdiegė [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="dfb29-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="dfb29-110">Sdk palaikančių programėlių sąrašą [rasite "Microsoft Intune" apsaugotose programėlėse](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="dfb29-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="dfb29-111">Strategijos taikomos po to, kai vartotojas, atitinkantis pirmiau nurodytus reikalavimus, prisijungia prie "Intune" SDK įgalintos programos.</span><span class="sxs-lookup"><span data-stu-id="dfb29-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="dfb29-112">Lengviausias būdas nustatyti, ar taikoma strategija, yra reikalavimas, kad vartotojas nustatytų kaištį strategijoje.</span><span class="sxs-lookup"><span data-stu-id="dfb29-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="dfb29-113">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="dfb29-113">For more information, see:</span></span>

[<span data-ttu-id="dfb29-114">APP/MAM trikčių šalinimo DUK</span><span class="sxs-lookup"><span data-stu-id="dfb29-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="dfb29-115">Kaip patvirtinti programos apsaugos strategijos nustatymą</span><span class="sxs-lookup"><span data-stu-id="dfb29-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="dfb29-116">Suprasti programos apsaugos strategijos pristatymo laiką</span><span class="sxs-lookup"><span data-stu-id="dfb29-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="dfb29-117">Kaip stebėti programų apsaugos strategijas</span><span class="sxs-lookup"><span data-stu-id="dfb29-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)