---
title: Ediscovery trikčių šalinimas turi klaidų
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676276"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="a4037-102">Ediscovery trikčių šalinimas turi klaidų</span><span class="sxs-lookup"><span data-stu-id="a4037-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="a4037-103">Kyla el. duomenų aptikimo problemų?</span><span class="sxs-lookup"><span data-stu-id="a4037-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="a4037-104">Toliau pateikiame keletą geriausios praktikos pavyzdžių:</span><span class="sxs-lookup"><span data-stu-id="a4037-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="a4037-105">Patikrinkite sulaikyto paskirstymo būseną.</span><span class="sxs-lookup"><span data-stu-id="a4037-105">Check the hold distribution status.</span></span>  <span data-ttu-id="a4037-106">Jei būsena yra **Įjungta (Laukiama)** arba **Išjungta (Laukiama)**, palaukite, kol bus baigtas sulaikytas paskirstymas.</span><span class="sxs-lookup"><span data-stu-id="a4037-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="a4037-107">Sulieti el. duomenų aptikimą turi naujinimus į vieną masinę užklausą, o ne pakartotinai atnaujinti kiekvienos operacijos strategiją.</span><span class="sxs-lookup"><span data-stu-id="a4037-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="a4037-108">Paleiskite Set-CaseHoldPolicy <policyname> -RetryDistribution" saugos ir atitikties centre "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="a4037-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="a4037-109">Daugiau informacijos [žr. Prisijungimas į Saugos & "PowerShell"](/powershell/exchange/connect-to-scc-powershell)atitikties centras .</span><span class="sxs-lookup"><span data-stu-id="a4037-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="a4037-110">Veiksmus, kaip patikrinti šiuos parametrus ir papildomą geriausią el. duomenų aptikimo švelninimo ir sprendimo praktiką, žr. [El. duomenų aptikimo sulaikymo klaidų trikčių šalinimas.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="a4037-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="a4037-111">Informacijos apie kitų dažnai pasitaikančių el. duomenų aptikimo trikčių diagnostiką žr. Dažniausiai pasitaikančių el. duomenų aptikimo problemų [ištyrimą, trikčių diagnostiką ir sprendimą.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="a4037-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
