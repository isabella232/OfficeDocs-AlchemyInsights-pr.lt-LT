---
title: "\"Microsoft Edge\" strategijos parametrų konfigūravimas \"Windows\""
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583738"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="db9fe-102">"Microsoft Edge" strategijos parametrų konfigūravimas "Windows"</span><span class="sxs-lookup"><span data-stu-id="db9fe-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="db9fe-103">Norėdami konfigūruoti strategijos parametrus ir valdomus naujinimus, skirtus "Microsoft Edge", naudokite grupės strategijos objektus (GPO).</span><span class="sxs-lookup"><span data-stu-id="db9fe-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="db9fe-104">Taip pat galite teikti politiką per registrą; tai tiktų (1) "Windows" įrenginiams, prijungtiems prie "Microsoft Active Directory" domeno ir (2) "Windows 10 Pro" ir įmonės egzemplioriams, kurie buvo įtraukti į "Microsoft Intune" įrenginių valdymą.</span><span class="sxs-lookup"><span data-stu-id="db9fe-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="db9fe-105">Norėdami sukonfigūruoti "Microsoft Edge" naudodami GPO, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="db9fe-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="db9fe-106">Prie grupės strategijos centrinės saugyklos, esančios "Active Directory" domene, arba atskirų kompiuterių strategijos apibrėžimo šablono aplanke, įdiekite visus administravimo šablonus, kurie įtraukia "Microsoft Edge" taisykles ir parametrus.</span><span class="sxs-lookup"><span data-stu-id="db9fe-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="db9fe-107">Konfigūruokite konkrečias strategijas, kurias norite nustatyti.</span><span class="sxs-lookup"><span data-stu-id="db9fe-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="db9fe-108">Jei norite sužinoti daugiau, skaitykite " [Microsoft Edge" strategijos parametrų konfigūravimas "Windows"](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="db9fe-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
