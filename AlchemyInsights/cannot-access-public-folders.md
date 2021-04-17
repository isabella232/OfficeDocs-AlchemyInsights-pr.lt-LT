---
title: Negalima pasiekti viešųjų aplankų
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819520"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="b4625-102">"Outlook" negali prisijungti prie viešųjų aplankų</span><span class="sxs-lookup"><span data-stu-id="b4625-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="b4625-103">Jei viešojo aplanko prieiga neveikia kai kuriems vartotojams, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="b4625-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="b4625-104">Prisijunkite prie EXO "PowerShell" ir sukonfigūruokite parametrą DefaultPublicFolderMailbox problemos vartotojo paskyroje, kad jis atitiktų darbingo vartotojo paskyros parametrą.</span><span class="sxs-lookup"><span data-stu-id="b4625-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="b4625-105">Pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="b4625-105">Example:</span></span>

<span data-ttu-id="b4625-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="b4625-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="b4625-107">Set-Mailbox ProblemaUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="b4625-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="b4625-108">Palaukite bent vieną valandą, kol pakeitimas įsigalios.</span><span class="sxs-lookup"><span data-stu-id="b4625-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="b4625-109">Jei problema išlieka, atlikite šią procedūrą ir [pašalinkite viešojo](https://aka.ms/pfcte) aplanko prieigos problemas naudodami "Outlook".</span><span class="sxs-lookup"><span data-stu-id="b4625-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="b4625-110">**Norėdami kontroliuoti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami "Outlook":**</span><span class="sxs-lookup"><span data-stu-id="b4625-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="b4625-111"><mailboxname>"Set-CASMailbox-PublicFolderClientAccess" $true arba "$false</span><span class="sxs-lookup"><span data-stu-id="b4625-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="b4625-112">$true: leisti vartotojams pasiekti viešuosius aplankus programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="b4625-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="b4625-113">$false: neleisti vartotojams pasiekti viešųjų aplankų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="b4625-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="b4625-114">– tai yra numatytoji reikšmė.</span><span class="sxs-lookup"><span data-stu-id="b4625-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="b4625-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="b4625-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="b4625-116">**Pastaba** Ši procedūra gali valdyti ryšius tik su "Outlook" darbalaukiu, skirta "Windows" klientams.</span><span class="sxs-lookup"><span data-stu-id="b4625-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="b4625-117">Vartotojas gali toliau pasiekti viešuosius aplankus naudodamas OWA arba "Outlook", skirtą "Mac".</span><span class="sxs-lookup"><span data-stu-id="b4625-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="b4625-118">Daugiau informacijos žr. ["Outlook" valdomi ryšiai su viešais aplankais valdomi palaikymo paskelbimas.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="b4625-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>