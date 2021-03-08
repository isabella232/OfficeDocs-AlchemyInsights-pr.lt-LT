---
title: Automatiškai šifruoti tam tikrus laiškus iš "Office 365"
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526757"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="4eee3-102">Automatiškai šifruoti tam tikrus laiškus iš "Office 365"</span><span class="sxs-lookup"><span data-stu-id="4eee3-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="4eee3-103">" [Exchange" administravimo centre](https://outlook.office365.com/ecp/)pasirinkite **pašto srauto > taisyklės**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="4eee3-104">Spustelėkite **naują (+)** piktogramą, tada spustelėkite taikyti "**Office 365" pranešimų šifravimą ir teisių apsaugą pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="4eee3-105">Dalyje **pavadinimas**, nurodykite taisyklės pavadinimą, pvz., *šifruoti visus el. laiškams*.</span><span class="sxs-lookup"><span data-stu-id="4eee3-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="4eee3-106">**Jei norite taikyti šią taisyklę, jei** pasirinksite **[taikyti visiems pranešimams]**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="4eee3-107">Prie lauko **atlikti** šį lauką spustelėkite **pasirinkti vieną**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="4eee3-108">Išplečiamajame meniu **RMS šablonas** pasirinkite **šifruoti**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="4eee3-109">(Jei nematote šios parinkties, vadinasi, jūsų planas neapima automatinio šifravimo.</span><span class="sxs-lookup"><span data-stu-id="4eee3-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="4eee3-110">Tačiau galite ją įtraukti!)</span><span class="sxs-lookup"><span data-stu-id="4eee3-110">But you can add it!)</span></span>
7. <span data-ttu-id="4eee3-111">Pažymėkite žymės langelį Tikrinti **šią taisyklę su svarbos lygiu** , tada pasirinkite norimą lygį.</span><span class="sxs-lookup"><span data-stu-id="4eee3-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="4eee3-112">Jei jūsų įmonė turi sutartinių įsipareigojimų išsiųsti visus laiškus užšifruotą, rekomenduojame nustatyti **aukštą** lygį.</span><span class="sxs-lookup"><span data-stu-id="4eee3-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="4eee3-113">Dalyje **pasirinkite šios taisyklės modelį** spustelėkite **įgalinti**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="4eee3-114">Pasirinkite bet kurią pasirinktinę parinktį (iš pasirinktinių pasirinkimų sąrašo, kurį galite atlikti šiuo metu, o daugelis iš jų gali būti paliekami numatytasis paprastumo parametras).</span><span class="sxs-lookup"><span data-stu-id="4eee3-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="4eee3-115">Spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="4eee3-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4eee3-116">Visada galite grįžti ir redaguoti šią taisyklę.</span><span class="sxs-lookup"><span data-stu-id="4eee3-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="4eee3-117">Daugiau informacijos apie šifravimo taisyklių kūrimą rasite [pašto srauto taisyklių nustatymas, kad būtų šifruojami el. laiškai "Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) "</span><span class="sxs-lookup"><span data-stu-id="4eee3-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

