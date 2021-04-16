---
title: Įvyko klaida, kai buvo įlaipinimo metu įkeliant kompiuterio analizės prieigos atpažinimo ženklo klaidą
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813696"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="6fe6e-102">Klaida "Įvyko klaida bandant nustatyti prieigos atpažinimo ženklą" naudojant kompiuterio "Analytics" parengimą</span><span class="sxs-lookup"><span data-stu-id="6fe6e-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="6fe6e-103">Ši klaida paprastai stebima pasibaigus autentifikavimo atpažinimo ženklo galiojimui.</span><span class="sxs-lookup"><span data-stu-id="6fe6e-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="6fe6e-104">Paprastai atnaujinant puslapį atnaujinamas atpažinimo ženklas.</span><span class="sxs-lookup"><span data-stu-id="6fe6e-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="6fe6e-105">Tačiau ši problema gali išlikti, jei paskyrai, naudojamai kompiuterio analizės sistemoje, taikomos sąlyginės prieigos strategijos.</span><span class="sxs-lookup"><span data-stu-id="6fe6e-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="6fe6e-106">"Azure" portale galite peržiūrėti "Azure AD" prisijungimo žurnalus, kad pamatytumėte, ar yra prisijungimo prie paskyros, kuri naudojama kompiuterio analizės parengimui, trikčių.</span><span class="sxs-lookup"><span data-stu-id="6fe6e-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="6fe6e-107">Daugiau informacijos apie sąlyginę prieigą rasite [Sąlyginės prieigos diegimo planas.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="6fe6e-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>