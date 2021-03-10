---
title: Nuomotojo strategijos taisymas (veiksmo nepaisymas)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695687"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="07640-102">Nuomotojo strategijos taisymas (veiksmo nepaisymas)</span><span class="sxs-lookup"><span data-stu-id="07640-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="07640-103">"Anti-spam" strategija jūsų nuomotojuje paveikė šį pranešimą.</span><span class="sxs-lookup"><span data-stu-id="07640-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="07640-104">Norėdami peržiūrėti strategiją, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="07640-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="07640-105">Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143), tada eikite į **grėsmių valdymo**  >  **strategija**  >  [apsauga nuo pašto šiukšlių](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="07640-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="07640-106">Patikrinkite, ar **strategijos šaltinis** nurodo:  **Add-XHeader/Modifysubject/peradresavimo/naikinimo/nėra veiksmų/BCC pranešimas**</span><span class="sxs-lookup"><span data-stu-id="07640-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="07640-107">Jei taip, skirtuke **Pasirinktinai** patikrinkite strategijos, kuri paveikė laišką, parametrus.</span><span class="sxs-lookup"><span data-stu-id="07640-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="07640-108">Gali būti, kad **standartiniai parametrai** , taikomi visiems "Exchange Online Protection" klientams, paveikė laišką.</span><span class="sxs-lookup"><span data-stu-id="07640-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="07640-109">Daugiau informacijos apie pašto šiukšlių filtravimo strategijų konfigūravimą rasite [pašto šiukšlių filtravimo strategijų](https://go.microsoft.com/fwlink/?linkid=2101431)konfigūravimas.</span><span class="sxs-lookup"><span data-stu-id="07640-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
