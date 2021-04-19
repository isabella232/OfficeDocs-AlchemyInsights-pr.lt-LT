---
title: Pasveikinimo pranešimas "Microsoft 365" grupėse
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
- "1200024"
- "5685"
ms.openlocfilehash: 6c46ba1b2c2c94e21d7c76e45df1d416ba423faf
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806414"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Pasveikinimo pranešimas "Microsoft 365" grupėse

Nauji vartotojai, prisijungiantys prie "Microsoft 365" grupės, gaus pasveikinimo el. laišką, jei ypatybė "UnifiedGroupWelcomeMessageEnabled" yra True.

Jei norite išjungti pasveikinimo pranešimą, naudokite šią [EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) komandą:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
