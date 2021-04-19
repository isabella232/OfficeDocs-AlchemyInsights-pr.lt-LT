---
title: "\"Office 365\" grupių arba komandų slėpimas arba slėpimas iš adresų sąrašo"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811464"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="b12cb-102">"Office 365" grupių arba komandų slėpimas arba slėpimas iš adresų sąrašo</span><span class="sxs-lookup"><span data-stu-id="b12cb-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="b12cb-103">Naudokite šią EXO "PowerShell" komandą, kad paslėptumėte arba atžymėtumėte "Office 365" grupę / komandas iš "Exchange" klientų ("Outlook", OWA) adresų sąrašų (GAL):</span><span class="sxs-lookup"><span data-stu-id="b12cb-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="b12cb-104">Naudokite šią EXO "PowerShell" komandą, kad paslėptumėte arba atžymėtumėte "Office365" grupę / komandas iš "Exchange" klientų ("Outlook", OWA):</span><span class="sxs-lookup"><span data-stu-id="b12cb-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="b12cb-105">Išsamias instrukcijas [žr. "Office 365" grupių slėpimas GAL ir "Exchange" klientuose.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)</span><span class="sxs-lookup"><span data-stu-id="b12cb-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
