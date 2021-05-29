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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702134"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="20625-102">Mikrodelsa arba ribojimas „Exchange Online PowerShell“</span><span class="sxs-lookup"><span data-stu-id="20625-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="20625-103">Kai „Exchange Online“ paleidžiate scenarijus ir „cmdlet“, galite matyti įspėjimus „Micro delay applied“ (taikoma mikrodelsa) arba delsą.</span><span class="sxs-lookup"><span data-stu-id="20625-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="20625-104">Štai keli pasiūlymai, kaip išspręsti šią problemą:</span><span class="sxs-lookup"><span data-stu-id="20625-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="20625-105">Paleiskite mūsų diagnostiką, kad atpalaidavę nuomotojo "PowerShell" sustojimo strategijas.</span><span class="sxs-lookup"><span data-stu-id="20625-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="20625-106">Šis sprendimas dažniausiai išspręs problemą.</span><span class="sxs-lookup"><span data-stu-id="20625-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="20625-107">Jei problema vis dar neišspręsta, [naudokite "Exchange Online v2" "PowerShell"](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)modulį, kuriame yra CMDlets, kurie pagrįsti REST API ir yra gerokai efektyvesni.</span><span class="sxs-lookup"><span data-stu-id="20625-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="20625-108">Tai gali būti puikus sprendimas daugeliui dažnai naudojamų „Get-CMDlet“.</span><span class="sxs-lookup"><span data-stu-id="20625-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="20625-109">Jei reikia naudoti CMDlets, kurios nėra įtrauktos į "v2" modulį, žr. ["PowerShell" cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)naudojimas dideliam "Office 365" vartotojų skaičius, kuriame kalbama apie tai, kaip pasiekti "PowerShell" apribojimų apribojimus "Exchange Online".</span><span class="sxs-lookup"><span data-stu-id="20625-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
