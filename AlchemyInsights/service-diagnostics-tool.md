---
title: Tarnybos diagnostikos įrankis, skirtas "Windows Virtual Desktop"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595866"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="47c91-102">Tarnybos diagnostikos įrankis, skirtas "Windows Virtual Desktop"</span><span class="sxs-lookup"><span data-stu-id="47c91-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="47c91-103">"Windows Virtual Desktop" (WVD) siūlo diagnostikos įrankį, kuris leidžia administratoriams identifikuoti klaidas naudojant vieną sąsają.</span><span class="sxs-lookup"><span data-stu-id="47c91-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="47c91-104">Šis įrankis registruoja su diagnostika susijusią informaciją, kai WVD naudoja kas nors, kam priskirtas WVD vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="47c91-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="47c91-105">Kiekviename žurnale yra informacija apie WVD vaidmenį, kuris dalyvauja veikloje, klaidų pranešimus, rodomus seanso metu, ir informaciją apie nuomotoją ir vartotoją.</span><span class="sxs-lookup"><span data-stu-id="47c91-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="47c91-106">"Azure Log Analytics" galima sukonfigūruoti užfiksuoti diagnostikos įrankio sukurtą veiklos žurnalą, atlikdami šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="47c91-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="47c91-107">Sukurkite žurnalo analizės darbo sritį naudodami ["Azure" portalą](https://go.microsoft.com/fwlink/?linkid=2129500) arba ["Azure PowerShell".](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="47c91-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="47c91-108">[Prijunkite "Windows" kompiuterius prie "Azure Monitor".](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="47c91-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="47c91-109">Gaukite darbo srities ID ir pirminį darbo srities raktą.</span><span class="sxs-lookup"><span data-stu-id="47c91-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="47c91-110">Sąrankos vediklis turi šią informaciją tinkamai sukonfigūruoti agentą ir užtikrinti, kad jis galėtų bendrauti su "Azure Monitor".</span><span class="sxs-lookup"><span data-stu-id="47c91-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="47c91-111">[Stumkite diagnostikos duomenis į savo darbo sritį.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="47c91-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="47c91-112">Galite stumti diagnostikos duomenis iš savo WVD nuomotojo į darbo srities žurnalo analizę.</span><span class="sxs-lookup"><span data-stu-id="47c91-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="47c91-113">[Nustatykite ir diagnozuokite](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemas, kurios yra vidinės arba išorinės WVD atžvilgiu.</span><span class="sxs-lookup"><span data-stu-id="47c91-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="47c91-114">Norėdami sužinoti daugiau apie WVD tarnybos diagnostikos įrankio konfigūravimą, žr. Žurnalo analizės naudojimas diagnostikos funkcijai.</span><span class="sxs-lookup"><span data-stu-id="47c91-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>