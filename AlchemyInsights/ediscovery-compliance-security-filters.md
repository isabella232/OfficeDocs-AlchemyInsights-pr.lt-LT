---
title: Per turinio paiešką/eksportavimą nepateikiami jokie rezultatai
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
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678681"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="774aa-102">Per turinio paiešką/eksportavimą nepateikiami jokie rezultatai</span><span class="sxs-lookup"><span data-stu-id="774aa-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="774aa-103">Jei kyla problemų dėl šių "elektroninės aptikimo" scenarijų:</span><span class="sxs-lookup"><span data-stu-id="774aa-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="774aa-104">Turinio ieška/eksportavimas pateikia duomenų arba netikėtų duomenų</span><span class="sxs-lookup"><span data-stu-id="774aa-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="774aa-105">"Udiscovery" ieška arba eksportavimas nepavyksta</span><span class="sxs-lookup"><span data-stu-id="774aa-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="774aa-106">Taip gali nutikti dėl tam tikrų atitikties saugos filtrų, kurie buvo sukonfigūruoti konkrečiame administratoriaus ir nebuvo perduoti visiems administratoriams.</span><span class="sxs-lookup"><span data-stu-id="774aa-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="774aa-107">Norėdami išspręsti šią problemą, patikrinkite, ar yra atitikties saugos filtrų, kurie gali sukelti šias problemas:</span><span class="sxs-lookup"><span data-stu-id="774aa-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="774aa-108">Prisijungimas prie saugos ir atitikties centro "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="774aa-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="774aa-109">Vykdykite šiuos commandlets:</span><span class="sxs-lookup"><span data-stu-id="774aa-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="774aa-110">Papildomos informacijos apie atitikties saugos filtrus ieškokite [turinio ieškos teisių filtravimas](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="774aa-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
