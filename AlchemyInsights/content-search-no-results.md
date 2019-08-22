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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516787"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="38a00-102">Jokių rezultatų iš turinio paieškos/eksportas</span><span class="sxs-lookup"><span data-stu-id="38a00-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="38a00-103">Problemos su turinio paieškos/eksporto negrįžta duomenis gali būti dėl tam tikrų atitikties saugos filtrą, kuris buvo setup iš konkrečių Admin ir nėra perduoti visi administratorių.</span><span class="sxs-lookup"><span data-stu-id="38a00-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="38a00-104">Norėdami išspręsti šią problemą, patikrinkite, ar yra bet atitikties saugos filtrus, kurie gali kelti tai:</span><span class="sxs-lookup"><span data-stu-id="38a00-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="38a00-105">Prisijungti prie saugos ir atitikties užtikrinimo centre "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="38a00-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="38a00-106">Vykdykite ir toliau "commandlet" komandas.</span><span class="sxs-lookup"><span data-stu-id="38a00-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="38a00-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="38a00-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="38a00-108">Gauti ComplianceSecurityFilter-organizacijos $org</span><span class="sxs-lookup"><span data-stu-id="38a00-108">Get-ComplianceSecurityFilter -Organization $org</span></span>