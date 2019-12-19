---
title: Atliekant darbalaukio "Analytics" sulaikymo metu įvyko klaida patvirtinant prieigos atpažinimo ženklo klaidą
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741226"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="91741-102">"Įvyko klaida patvirtinant prieigos žetonas" klaida per Desktop Analytics supažindinimo</span><span class="sxs-lookup"><span data-stu-id="91741-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="91741-103">Ši klaida paprastai pastebima, kai baigiasi autentifikavimo atpažinimo ženklo galiojimo laikas.</span><span class="sxs-lookup"><span data-stu-id="91741-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="91741-104">Paprastai, gaivus puslapį atnaujina atpažinimo ženklas.</span><span class="sxs-lookup"><span data-stu-id="91741-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="91741-105">Tačiau ši problema gali tęstis, jei yra sąlyginis prieigos strategijos taikomos sąskaitos naudojamas borto darbalaukio analizė.</span><span class="sxs-lookup"><span data-stu-id="91741-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="91741-106">Galite peržiūrėti Azure AD prisijungti žurnalus Azure portale Norėdami pamatyti, jei yra kokių nors prisijungimo nesėkmių paskyros naudojama Desktop Analytics parengimas.</span><span class="sxs-lookup"><span data-stu-id="91741-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="91741-107">Jei turite daugiau informacijos apie sąlyginę prieigą, apsilankykite ["sąlyginės prieigos" diegimo planavimas](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="91741-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>