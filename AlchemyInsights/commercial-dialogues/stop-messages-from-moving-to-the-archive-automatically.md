---
title: Automatinis pranešimas, kad automatiškai pereitumėte prie archyvo
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749827"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="63b16-102">Automatinis pranešimas, kad automatiškai pereitumėte prie archyvo</span><span class="sxs-lookup"><span data-stu-id="63b16-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="63b16-103">Jei naudojate saugojimo strategiją, galite pakeisti tos strategijos saugojimo amžių, kad laiškai nebūtų archyvuojami automatiškai.</span><span class="sxs-lookup"><span data-stu-id="63b16-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="63b16-104">Toliau nurodyta, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="63b16-104">Here's how:</span></span>

1. <span data-ttu-id="63b16-105">" [Exchange" administravimo centre](https://go.microsoft.com/fwlink/?linkid=2059104)pasirinkite **atitikties valdymo**  >  **išsaugojimo žymės**.</span><span class="sxs-lookup"><span data-stu-id="63b16-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="63b16-106">Raskite savo perkėlimą į archyvo saugojimo žymę.</span><span class="sxs-lookup"><span data-stu-id="63b16-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="63b16-107">Dalyje saugojimo žymė pakeiskite saugojimo laikotarpį (archyvo laikotarpis), kad **niekada** nesustabdytumėte elementų automatiškai suarchyvuotų pagal saugojimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="63b16-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="63b16-108">Taip pakeisite visų pašto dėžučių archyvo parametrą, kuriam taikoma ši saugojimo žymė.</span><span class="sxs-lookup"><span data-stu-id="63b16-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
