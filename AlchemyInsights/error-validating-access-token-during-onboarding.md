---
title: Įvyko klaida tikrinant "Access" atpažinimo ženklo klaidą atliekant "Desktop Analytics" įlipimo metu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783559"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="d4c55-102">"Įvyko klaida tikrinant prieigos žetoną" klaida atliekant darbalaukio analizės parengimo paslaugą</span><span class="sxs-lookup"><span data-stu-id="d4c55-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="d4c55-103">Ši klaida paprastai stebima, kai baigiasi autentifikavimo atpažinimo ženklas.</span><span class="sxs-lookup"><span data-stu-id="d4c55-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="d4c55-104">Paprastai atnaujinti puslapį atnaujina atpažinimo ženklą.</span><span class="sxs-lookup"><span data-stu-id="d4c55-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="d4c55-105">Tačiau ši problema gali tęstis, jei yra sąlyginės prieigos strategijos, pritaikytos paskyrai, kuri naudojama kompiuterio analizei laive.</span><span class="sxs-lookup"><span data-stu-id="d4c55-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="d4c55-106">Galite peržiūrėti "Azure AD" prisijungimo žurnalus, esančius "Azure" portale, Norėdami sužinoti, ar yra kokių nors prisijungimo prie kompiuterio "Analytics" parengimo naudojamo abonemento klaidų.</span><span class="sxs-lookup"><span data-stu-id="d4c55-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="d4c55-107">Daugiau informacijos apie [sąlyginę prieigą rasite savo sąlyginės prieigos diegimo planavimas](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="d4c55-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>