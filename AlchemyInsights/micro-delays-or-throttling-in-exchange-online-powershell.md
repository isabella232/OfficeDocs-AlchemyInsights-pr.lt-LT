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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314708"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikrodelsa arba ribojimas „Exchange Online PowerShell“

Kai „Exchange Online“ paleidžiate scenarijus ir „cmdlet“, galite matyti įspėjimus „Micro delay applied“ (taikoma mikrodelsa) arba delsą. Štai keli pasiūlymai, kaip išspręsti šią problemą:

- Paleiskite mūsų diagnostiką, kad atpalaidavę nuomotojo "PowerShell" sustojimo strategijas. Šis sprendimas padės išspręsti šią problemą daugumai.
- Jei problema vis dar neišspręsta, naudokite ["Exchange Online v2" "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modulį, kuriame yra CMDlets, kurie pagrįsti REST API ir yra gerokai efektyvesni. Tai gali būti puikus sprendimas daugeliui dažnai naudojamų „Get-CMDlet“.
- Jei reikia naudoti CMDlets, kurios nėra įtrauktos į "v2" modulį, žr. ["PowerShell" cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)naudojimas dideliam "Office 365" vartotojų skaičius, kuriame kalbama apie tai, kaip pasiekti "PowerShell" apribojimų apribojimus "Exchange Online".
