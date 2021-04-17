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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="a3569-102">Mikrodelsa arba ribojimas „Exchange Online PowerShell“</span><span class="sxs-lookup"><span data-stu-id="a3569-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="a3569-103">Kai „Exchange Online“ paleidžiate scenarijus ir „cmdlet“, galite matyti įspėjimus „Micro delay applied“ (taikoma mikrodelsa) arba delsą.</span><span class="sxs-lookup"><span data-stu-id="a3569-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="a3569-104">Štai du su tuo susiję pasiūlymai:</span><span class="sxs-lookup"><span data-stu-id="a3569-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="a3569-105">Galite pabandyti naudoti [„Exchange Online“ v2 „PowerShell“ modulį](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), apimantį „CMDlet“, kurie yra pagrįsti REST API ir gerokai efektyvesni.</span><span class="sxs-lookup"><span data-stu-id="a3569-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="a3569-106">Tai gali būti puikus sprendimas daugeliui dažnai naudojamų „Get-CMDlet“.</span><span class="sxs-lookup"><span data-stu-id="a3569-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="a3569-107">Jei jums reikia naudoti „CMDlet“, kurios dar neįtrauktos į v2 modulį, žr. [„PowerShell“ „cmdlet“ vykdymas dideliam „Office 365“ vartotojų skaičiui](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), kur kalbama apie tai, kaip elgtis su numatomais „PowerShell“ ribojimo limitais „Exchange Online“.</span><span class="sxs-lookup"><span data-stu-id="a3569-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
