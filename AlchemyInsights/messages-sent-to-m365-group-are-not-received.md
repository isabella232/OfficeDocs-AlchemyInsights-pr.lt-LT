---
title: „Microsoft 365“ grupei siunčiamus pranešimus gauna ne visi nariai
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823795"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>„Microsoft 365“ grupei siunčiamus pranešimus gauna ne visi nariai

Įsitikinkite, kad visi grupės nariai užsiprenumeravo gauti el. laiškus. Žr. [Stebėti grupę programoje „Outlook“](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Norėdami patikrinti narių, kurie užsiprenumeravo grupės el. laiškus, pranešimų būseną, paleiskite toliau pateiktą komandą naudodami [„EXO PowerShell“](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Naudodami šią „EXO PowerShell“ komandą sukonfigūruokite, kad visi grupės nariai savo aplankuose Gauta gautų el. laiškus, siunčiamus „Microsoft 365“ grupei:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Toliau pateikiami pavyzdžiai.

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`