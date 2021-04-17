---
title: Mikrodelsa arba ribojimas „Exchange Online PowerShell“
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
- "3500011"
- "5106"
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830041"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrodelsa arba ribojimas „Exchange Online PowerShell“

Kai „Exchange Online“ paleidžiate scenarijus ir „cmdlet“, galite matyti įspėjimus „Micro delay applied“ (taikoma mikrodelsa) arba delsą. Štai du su tuo susiję pasiūlymai:

- Galite pabandyti naudoti [„Exchange Online“ v2 „PowerShell“ modulį](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), apimantį „CMDlet“, kurie yra pagrįsti REST API ir gerokai efektyvesni. Tai gali būti puikus sprendimas daugeliui dažnai naudojamų „Get-CMDlet“.
- Jei jums reikia naudoti „CMDlet“, kurios dar neįtrauktos į v2 modulį, žr. [„PowerShell“ „cmdlet“ vykdymas dideliam „Office 365“ vartotojų skaičiui](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), kur kalbama apie tai, kaip elgtis su numatomais „PowerShell“ ribojimo limitais „Exchange Online“.
