---
title: Ryšių strategijos taisymas
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
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695894"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="7db9e-102">Ryšių strategijos taisymas</span><span class="sxs-lookup"><span data-stu-id="7db9e-102">Fix connection policy</span></span>

<span data-ttu-id="7db9e-103">Laiškas buvo pažymėtas saugiomis ir pristatytas į vartotojo aplanką Gauta, nes siuntimo IP adresas buvo pažymėtas saugiomis ryšių filtravimo strategijoje.</span><span class="sxs-lookup"><span data-stu-id="7db9e-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="7db9e-104">Norėdami peržiūrėti strategiją, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="7db9e-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="7db9e-105">Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143), tada eikite į **grėsmių valdymo**  >  **strategija**  >  [apsauga nuo pašto šiukšlių](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="7db9e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="7db9e-106">Skirtuke **Pasirinktinai** pasirinkite **jungimosi filtro strategiją**, tada pasirinkite **Redaguoti strategiją**.</span><span class="sxs-lookup"><span data-stu-id="7db9e-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="7db9e-107">Peržiūrėkite **IP leidžiamųjų** sąrašą.</span><span class="sxs-lookup"><span data-stu-id="7db9e-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="7db9e-108">Sužinokite, ar įgalintas **saugus sąrašas** .</span><span class="sxs-lookup"><span data-stu-id="7db9e-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="7db9e-109">"Microsoft" prenumeroja trečiųjų šalių patikimų siuntėjų šaltinius.</span><span class="sxs-lookup"><span data-stu-id="7db9e-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="7db9e-110">Jei įgalintas **saugus sąrašas** , šie Patikimi siuntėjai nėra klaidingai pažymėti kaip šlamštas.</span><span class="sxs-lookup"><span data-stu-id="7db9e-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="7db9e-111">Rekomenduojame pasirinkti šią parinktį, nes ji sumažins neteisingus teigiamus rezultatus (gerą paštą, kuris klasifikuojamas kaip šlamštas), kurį gaunate.</span><span class="sxs-lookup"><span data-stu-id="7db9e-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
