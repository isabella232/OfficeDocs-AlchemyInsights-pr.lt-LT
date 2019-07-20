---
title: Turinio paieška jokių rezultatų
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800474"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="811a2-102">Jokių rezultatų iš turinio paieškos/eksportas</span><span class="sxs-lookup"><span data-stu-id="811a2-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="811a2-103">Problemos su turinio paieškos/eksporto negrįžta duomenis gali būti dėl tam tikrų atitikties saugos filtrą, kuris buvo setup iš konkrečių Admin ir nėra perduoti visi administratorių.</span><span class="sxs-lookup"><span data-stu-id="811a2-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="811a2-104">Norėdami išspręsti šią problemą, patikrinkite, ar yra bet atitikties saugos filtrus, kurie gali kelti tai:</span><span class="sxs-lookup"><span data-stu-id="811a2-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="811a2-105">Prisijungti prie saugos ir atitikties užtikrinimo centre "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="811a2-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="811a2-106">Vykdykite ir toliau "commandlet" komandas.</span><span class="sxs-lookup"><span data-stu-id="811a2-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="811a2-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="811a2-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="811a2-108">Gauti ComplianceSecurityFilter-organizacijos $org</span><span class="sxs-lookup"><span data-stu-id="811a2-108">Get-ComplianceSecurityFilter -Organization $org</span></span>