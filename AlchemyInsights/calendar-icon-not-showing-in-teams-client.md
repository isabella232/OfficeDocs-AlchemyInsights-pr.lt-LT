---
title: Kalendoriaus piktograma nerodo „Teams“ kliento
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819961"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="0349e-102">Kalendoriaus piktograma nerodo „Teams“ kliento</span><span class="sxs-lookup"><span data-stu-id="0349e-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="0349e-103">„Teams“ kalendoriaus skirtukui būtina prieiga prie „Exchange“ pašto dėžutės naudojant „Exchange Web Services“.</span><span class="sxs-lookup"><span data-stu-id="0349e-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="0349e-104">„Exchange“ pašto dėžutė gali būti internetinė arba vietinė.</span><span class="sxs-lookup"><span data-stu-id="0349e-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="0349e-105">Interneto vartotojai, kurie nemato kalendoriaus skirtuko, turi įsitikinti, kad jie yra [licencijuoti „Exchange Online“ pašto dėžutei ir pašto dėžutė yra įgalinta](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="0349e-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="0349e-106">Jei vartotojas turi tinkamą pašto dėžutę „Exchange Online“, tačiau vis tiek nemato kalendoriaus skirtuko, gali būti, kad kilo tinklo problemų.</span><span class="sxs-lookup"><span data-stu-id="0349e-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="0349e-107">Naudokite [„Microsoft“ nuotolinio ryšio analizatorių](https://testconnectivity.microsoft.com/) ir paveiktam vartotojui atlikite **„Microsoft Exchange“ žiniatinklio tarnybų ryšio testus**.</span><span class="sxs-lookup"><span data-stu-id="0349e-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="0349e-108">Galiausiai patikrinkite [„Teams“ programų sąrankos strategijas](https://admin.teams.microsoft.com/policies/app-setup), kad įsitikintumėte, jog kalendoriaus programa nebuvo pašalinta iš vartotojui taikomos strategijos (greičiausiai tai **visuotinis (visos organizacijos numatytasis nustatymas)**.</span><span class="sxs-lookup"><span data-stu-id="0349e-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="0349e-109">Jei vartotojai veikia vietoje, būtina įsitikinti, kad hibridinė konfigūracija yra tinkama.</span><span class="sxs-lookup"><span data-stu-id="0349e-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="0349e-110">Triktims šalinti naudokite [hibridinės konfigūracijos vediklį](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="0349e-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="0349e-111">Atkreipkite dėmesį, kad [„Teams“ būtina „Exchange 2016“ CU3 ar naujesnė versija](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="0349e-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
