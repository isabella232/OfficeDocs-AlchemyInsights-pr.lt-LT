---
title: Kalendoriaus piktograma nerodo „Teams“ kliento
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932201"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="f1987-102">Kalendoriaus piktograma nerodo „Teams“ kliento</span><span class="sxs-lookup"><span data-stu-id="f1987-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="f1987-103">„Teams“ kalendoriaus skirtukui būtina prieiga prie „Exchange“ pašto dėžutės naudojant „Exchange Web Services“.</span><span class="sxs-lookup"><span data-stu-id="f1987-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="f1987-104">„Exchange“ pašto dėžutė gali būti internetinė arba vietinė.</span><span class="sxs-lookup"><span data-stu-id="f1987-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="f1987-105">Interneto vartotojai, kurie nemato kalendoriaus skirtuko, turi įsitikinti, kad jie yra [licencijuoti „Exchange Online“ pašto dėžutei ir pašto dėžutė yra įgalinta](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="f1987-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="f1987-106">Jei vartotojas turi tinkamą pašto dėžutę „Exchange Online“, tačiau vis tiek nemato kalendoriaus skirtuko, gali būti, kad kilo tinklo problemų.</span><span class="sxs-lookup"><span data-stu-id="f1987-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="f1987-107">Naudokite [„Microsoft“ nuotolinio ryšio analizatorių](https://testconnectivity.microsoft.com/) ir paveiktam vartotojui atlikite **„Microsoft Exchange“ žiniatinklio tarnybų ryšio testus**.</span><span class="sxs-lookup"><span data-stu-id="f1987-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="f1987-108">Galiausiai patikrinkite [„Teams“ programų sąrankos strategijas](https://admin.teams.microsoft.com/policies/app-setup), kad įsitikintumėte, jog kalendoriaus programa nebuvo pašalinta iš vartotojui taikomos strategijos (greičiausiai tai **visuotinis (visos organizacijos numatytasis nustatymas)**.</span><span class="sxs-lookup"><span data-stu-id="f1987-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="f1987-109">Jei vartotojai veikia vietoje, būtina įsitikinti, kad hibridinė konfigūracija yra tinkama.</span><span class="sxs-lookup"><span data-stu-id="f1987-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="f1987-110">Triktims šalinti naudokite [hibridinės konfigūracijos vediklį](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="f1987-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="f1987-111">Atkreipkite dėmesį, kad [„Teams“ būtina „Exchange 2016“ CU3 ar naujesnė versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="f1987-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
