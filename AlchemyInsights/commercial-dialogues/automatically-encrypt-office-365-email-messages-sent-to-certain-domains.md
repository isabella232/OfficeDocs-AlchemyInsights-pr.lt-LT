---
title: Automatinis "Office 365" el. laiškų, siunčiamų į tam tikrus domenus, šifravimas
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749307"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="abd72-102">Automatinis "Office 365" el. laiškų, siunčiamų į tam tikrus domenus, šifravimas</span><span class="sxs-lookup"><span data-stu-id="abd72-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="abd72-103">" [Exchange" administravimo centre](https://outlook.office365.com/ecp/)pasirinkite **pašto srauto > taisyklės**.</span><span class="sxs-lookup"><span data-stu-id="abd72-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="abd72-104">Spustelėkite **naują (+)** piktogramą, tada spustelėkite taikyti "**Office 365" pranešimų šifravimą ir teisių apsaugą pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="abd72-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="abd72-105">Dalyje **pavadinimas** įveskite taisyklės pavadinimą, pvz., šifruoti " *contoso.com" siunčiamus pranešimams*.</span><span class="sxs-lookup"><span data-stu-id="abd72-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="abd72-106">**Jei norite taikyti šią taisyklę**, pasirinkite **gavėją > domenas**.</span><span class="sxs-lookup"><span data-stu-id="abd72-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="abd72-107">Įvesti domeno vardą, pvz., **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="abd72-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="abd72-108">Spustelėkite piktogramą **įtraukti (+)** , tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="abd72-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="abd72-109">Prie lauko **atlikti** šį lauką spustelėkite **pasirinkti vieną**.</span><span class="sxs-lookup"><span data-stu-id="abd72-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="abd72-110">Išplečiamajame meniu **RMS šablonas** pasirinkite **šifruoti**, tada spustelėkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="abd72-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="abd72-111">(Jei nematote šios parinkties, vadinasi, jūsų planas neapima automatinio šifravimo.</span><span class="sxs-lookup"><span data-stu-id="abd72-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="abd72-112">Tačiau galite ją įtraukti!)</span><span class="sxs-lookup"><span data-stu-id="abd72-112">But you can add it!)</span></span>
9. <span data-ttu-id="abd72-113">Pasirinkite bet kurią pasirinktinę parinktį (iš pasirinktinių pasirinkimų sąrašo, kurį galite atlikti šiuo metu, o daugelis iš jų gali būti paliekami numatytasis paprastumo parametras).</span><span class="sxs-lookup"><span data-stu-id="abd72-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="abd72-114">Spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="abd72-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="abd72-115">Visada galite grįžti ir redaguoti šią taisyklę.</span><span class="sxs-lookup"><span data-stu-id="abd72-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="abd72-116">Daugiau informacijos apie šifravimo taisyklių kūrimą rasite [pašto srauto taisyklių nustatymas, kad būtų šifruojami el. laiškai "Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) "</span><span class="sxs-lookup"><span data-stu-id="abd72-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>