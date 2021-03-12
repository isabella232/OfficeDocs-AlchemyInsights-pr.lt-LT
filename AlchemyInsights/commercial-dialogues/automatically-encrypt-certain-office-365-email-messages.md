---
title: Automatinis tam tikrų "Office 365" laiškų šifravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749438"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="e248f-102">Automatinis tam tikrų "Office 365" laiškų šifravimas</span><span class="sxs-lookup"><span data-stu-id="e248f-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="e248f-103">Galite automatiškai šifruoti laišką, kurį vartotojai siunčia tam tikriems išoriniams žmonėms arba organizacijoms.</span><span class="sxs-lookup"><span data-stu-id="e248f-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="e248f-104">Norėdami tai atlikti, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="e248f-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="e248f-105">" [Exchange" administravimo centre](https://outlook.office365.com/ecp/)pasirinkite **pašto srauto > taisyklės**.</span><span class="sxs-lookup"><span data-stu-id="e248f-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="e248f-106">Spustelėkite **naują (+)** piktogramą, tada spustelėkite taikyti "**Office 365" pranešimų šifravimą ir teisių apsaugą pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="e248f-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="e248f-107">Dalyje **pavadinimas** įveskite taisyklės pavadinimą, pvz., šifruoti " *DrToniRamos@gmail.com" siunčiamus pranešimams*.</span><span class="sxs-lookup"><span data-stu-id="e248f-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="e248f-108">**Jei norite taikyti šią taisyklę**, pasirinkite **gavėją > yra šis asmuo**.</span><span class="sxs-lookup"><span data-stu-id="e248f-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="e248f-109">Lange **Pasirinkti narius** pasirinkite asmens, kuriam norite taikyti šifravimo taisyklę, vardą, tada spustelėkite **įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="e248f-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="e248f-110">Baigę įtraukti vartotojų, spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="e248f-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="e248f-111">Prie lauko **atlikti** šį lauką spustelėkite **pasirinkti vieną**.</span><span class="sxs-lookup"><span data-stu-id="e248f-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="e248f-112">Išplečiamajame meniu **RMS šablonas** pasirinkite **šifruoti**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="e248f-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="e248f-113">(Jei nematote šios parinkties, vadinasi, jūsų planas neapima automatinio šifravimo.</span><span class="sxs-lookup"><span data-stu-id="e248f-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="e248f-114">Tačiau galite ją įtraukti!)</span><span class="sxs-lookup"><span data-stu-id="e248f-114">But you can add it!)</span></span>
9. <span data-ttu-id="e248f-115">Pasirinkite bet kurią pasirinktinę parinktį (iš pasirinktinių pasirinkimų sąrašo, kurį galite atlikti šiuo metu, o daugelis iš jų gali būti paliekami numatytasis paprastumo parametras).</span><span class="sxs-lookup"><span data-stu-id="e248f-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="e248f-116">Spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="e248f-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e248f-117">Visada galite grįžti ir redaguoti šią taisyklę.</span><span class="sxs-lookup"><span data-stu-id="e248f-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="e248f-118">Daugiau informacijos apie šifravimo taisyklių kūrimą rasite [pašto srauto taisyklių nustatymas, kad būtų šifruojami el. laiškai "Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)".</span><span class="sxs-lookup"><span data-stu-id="e248f-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

