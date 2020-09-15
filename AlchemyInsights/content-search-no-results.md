---
title: Turinio ieškos rezultatų nėra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680655"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="ea137-102">Nėra rezultatų iš turinio ieškos/eksportavimo</span><span class="sxs-lookup"><span data-stu-id="ea137-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="ea137-103">Problemos dėl turinio ieškos/eksportavimo negrąžinant jokių duomenų gali būti dėl tam tikro atitikties saugos filtro, kurį nustatė konkretus administratorius, o ne visiems administratoriams.</span><span class="sxs-lookup"><span data-stu-id="ea137-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="ea137-104">Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="ea137-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="ea137-105">Prisijungimas prie saugos ir atitikties centro "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="ea137-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ea137-106">Vykdykite šiuos commandlets:</span><span class="sxs-lookup"><span data-stu-id="ea137-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="ea137-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="ea137-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="ea137-108">Gauti – ComplianceSecurityFilter – organizacijos $org</span><span class="sxs-lookup"><span data-stu-id="ea137-108">Get-ComplianceSecurityFilter -Organization $org</span></span>