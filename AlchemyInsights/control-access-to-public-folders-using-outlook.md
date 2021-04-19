---
title: Prieigos prie viešųjų aplankų valdymas naudojant "Outlook"
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816748"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="6baed-102">Prieigos prie viešųjų aplankų valdymas naudojant "Outlook"</span><span class="sxs-lookup"><span data-stu-id="6baed-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="6baed-103">Norėdami kontroliuoti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami "Outlook":</span><span class="sxs-lookup"><span data-stu-id="6baed-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="6baed-104">Naudoti `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="6baed-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="6baed-105">$true: leisti vartotojams pasiekti viešuosius aplankus programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="6baed-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="6baed-106">$false: neleisti vartotojams pasiekti viešųjų aplankų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="6baed-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="6baed-107">– tai yra numatytoji reikšmė.</span><span class="sxs-lookup"><span data-stu-id="6baed-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="6baed-108">Pastaba: ši procedūra gali valdyti tik ryšius su "Outlook" darbalaukiu, skirta "Windows" klientams.</span><span class="sxs-lookup"><span data-stu-id="6baed-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="6baed-109">Vartotojai gali toliau pasiekti viešuosius aplankus naudodami OWA arba "Outlook", skirtą "Mac".</span><span class="sxs-lookup"><span data-stu-id="6baed-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="6baed-110">Daugiau informacijos žr. ["Outlook" valdomi ryšiai](https://aka.ms/controlpf) su viešais aplankais.</span><span class="sxs-lookup"><span data-stu-id="6baed-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
