---
title: Prenumeratų prieiga
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807715"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="979a1-102">Nepavyksta prisijungti prie "Azure" dėl naršyklės problemų (naršyklė stringa, išlaiko verpimą, neįkeliamas ir kt.)</span><span class="sxs-lookup"><span data-stu-id="979a1-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="979a1-103">Jums gali turėti įtakos.</span><span class="sxs-lookup"><span data-stu-id="979a1-103">You might be impacted by an outage.</span></span> <span data-ttu-id="979a1-104">Patikrinkite, ar yra nevykdomas "outage": " [Azure Health" būsena](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="979a1-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="979a1-105">Išeikite iš visų aktyvių "Azure" seansų.</span><span class="sxs-lookup"><span data-stu-id="979a1-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="979a1-106">Paleiskite savo žiniatinklio naršyklės privatų arba inkognito režimą.</span><span class="sxs-lookup"><span data-stu-id="979a1-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="979a1-107">Taip pat galite pabandyti atnaujinti naršyklę, naudoti kitą naršyklę, panaikinti talpyklos slapukus, jei aukščiau neveikia.</span><span class="sxs-lookup"><span data-stu-id="979a1-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="979a1-108">Sužinokite daugiau: [prisijungimo problemų šalinimas](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="979a1-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="979a1-109">**Nepavyksta pasiekti prenumeratų**</span><span class="sxs-lookup"><span data-stu-id="979a1-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="979a1-110">Įsitikinkite, kad " [Azure" portale](https://portal.azure.com/), viršutiniame dešiniajame kampe pažymėta teisinga "Azure" katalogas.</span><span class="sxs-lookup"><span data-stu-id="979a1-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="979a1-111">" [Azure" paskyros centre](https://account.windowsazure.com/Subscriptions)įsitikinkite, kad abonementas, kurį naudoja paskyros administratorius.</span><span class="sxs-lookup"><span data-stu-id="979a1-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="979a1-112">Sužinokite daugiau: [rastų prenumeratų trikčių diagnostika](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="979a1-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="979a1-113">**Negalima pasiekti atsiskaitymo retrospektyvos**</span><span class="sxs-lookup"><span data-stu-id="979a1-113">**Unable to access billing history**</span></span>

<span data-ttu-id="979a1-114">Abonemento administratorius turi užtikrinti, kad vartotojas, turintis prieigą prie atsiskaitymo informacijos, būtų įtrauktas į "Azure Active Directory" kaip svečias: [pridėti arba naikinti naują vartotoją](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="979a1-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="979a1-115">Vartotojui tada turi būti suteiktas visuotinio administratoriaus vaidmuo: [priskirti vaidmenį vartotojams](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="979a1-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="979a1-116">Paskelbkite šį vartotoją, vartotojas gali teikti atsiskaitymo prieigą naudodamas RBAC strategiją: [suteikti prieigą prie atsiskaitymo](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="979a1-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="979a1-117">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="979a1-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="979a1-118">Negaliu prisijungti prie savo "Azure" prenumeratos valdymo</span><span class="sxs-lookup"><span data-stu-id="979a1-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)