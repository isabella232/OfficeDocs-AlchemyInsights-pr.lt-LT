---
title: "\"Windows Virtual Desktop\" tarnybos diagnostikos įrankis"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678625"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="e1fd6-102">"Windows Virtual Desktop" tarnybos diagnostikos įrankis</span><span class="sxs-lookup"><span data-stu-id="e1fd6-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="e1fd6-103">"Windows Virtual Desktop" (WVD) siūlo diagnostikos įrankį, leidžiantį administratoriams nustatyti klaidas per vieną sąsają.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="e1fd6-104">Šiame įrankyje yra su diagnostika susijusi informacija, kai "WVD" naudoja kas nors priskyrė "WVD" vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="e1fd6-105">Kiekviename logaritme yra informacijos apie "WVD" vaidmenį, susijusį su veikla, seanso metu rodomus klaidų pranešimus ir informaciją apie nuomotoją ir vartotoją.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="e1fd6-106">"Azure" žurnalų analizės galima sukonfigūruoti, kad būtų užfiksuoti veiklos registras, sukurtas diagnostikos įrankiu.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="e1fd6-107">Toliau nurodyta, kaip tai padaryti.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-107">Here's how:</span></span>

1. <span data-ttu-id="e1fd6-108">Sukurkite žurnalų analizės darbo sritį naudodami " [Azure" portalą](https://go.microsoft.com/fwlink/?linkid=2129500) arba " [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)".</span><span class="sxs-lookup"><span data-stu-id="e1fd6-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="e1fd6-109">[Prijunkite "Windows" kompiuterius prie "Azure Monitor"](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="e1fd6-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="e1fd6-110">Gauti darbo srities ID ir savo darbo srities pirminį raktą.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="e1fd6-111">Sąrankos vediklyje reikia šios informacijos, kad būtų galima tinkamai sukonfigūruoti agentą ir užtikrinti, kad jis galėtų bendrauti su "Azure Monitor".</span><span class="sxs-lookup"><span data-stu-id="e1fd6-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="e1fd6-112">[Paspauskite diagnostikos duomenis į darbo sritį](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="e1fd6-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="e1fd6-113">Galite stumti diagnostikos duomenis iš savo "WVD" nuomotojo prie savo darbo srities žurnalų analizės.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="e1fd6-114">[Identifikuoti ir diagnozuoti](https://go.microsoft.com/fwlink/?linkid=2128338) vidines arba išorines problemas, susijusias su wvd.</span><span class="sxs-lookup"><span data-stu-id="e1fd6-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="e1fd6-115">Jei norite sužinoti daugiau apie "WVD" paslaugų diagnostikos įrankio konfigūravimą, žiūrėkite [diagnostikos funkcijai naudokite žurnalų analizės funkciją](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="e1fd6-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
