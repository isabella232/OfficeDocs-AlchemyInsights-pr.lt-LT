---
title: Mikrodelsa arba ribojimas „Exchange Online PowerShell“
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947906"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrodelsa arba ribojimas „Exchange Online PowerShell“

Kai „Exchange Online“ paleidžiate scenarijus ir „cmdlet“, galite matyti įspėjimus „Micro delay applied“ (taikoma mikrodelsa) arba delsą. Štai du su tuo susiję pasiūlymai:

- Galite pabandyti naudoti [„Exchange Online“ v2 „PowerShell“ modulį](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), apimantį „CMDlet“, kurie yra pagrįsti REST API ir gerokai efektyvesni. Tai gali būti puikus sprendimas daugeliui dažnai naudojamų „Get-CMDlet“.
- Jei jums reikia naudoti „CMDlet“, kurios dar neįtrauktos į v2 modulį, žr. [„PowerShell“ „cmdlet“ vykdymas dideliam „Office 365“ vartotojų skaičiui](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), kur kalbama apie tai, kaip elgtis su numatomais „PowerShell“ ribojimo limitais „Exchange Online“.
