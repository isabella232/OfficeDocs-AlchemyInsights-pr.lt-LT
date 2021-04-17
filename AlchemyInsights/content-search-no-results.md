---
title: Turinio ieška be rezultatų
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816856"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="1c439-102">Nėra rezultatų iš turinio ieškos / eksporto</span><span class="sxs-lookup"><span data-stu-id="1c439-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="1c439-103">Turinio ieškos / eksporto problemos, kurios negrąžina jokių duomenų, gali būti dėl tam tikro atitikties saugos filtro, kurį buvo sąranka konkretaus administratoriaus, o ne perduoti visiems administratoriams.</span><span class="sxs-lookup"><span data-stu-id="1c439-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="1c439-104">Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šią problemą:</span><span class="sxs-lookup"><span data-stu-id="1c439-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="1c439-105">Prisijungimas prie saugos ir atitikties centro "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="1c439-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="1c439-106">Vykdykite šias komandas:</span><span class="sxs-lookup"><span data-stu-id="1c439-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="1c439-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="1c439-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="1c439-108">Get-ComplianceSecurityFilter organizacijos $org</span><span class="sxs-lookup"><span data-stu-id="1c439-108">Get-ComplianceSecurityFilter -Organization $org</span></span>