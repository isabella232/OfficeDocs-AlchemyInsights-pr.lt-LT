---
title: Negalima pasiekti viešųjų aplankų
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341411"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="aa546-102">"Outlook" negali prisijungti prie viešųjų aplankų</span><span class="sxs-lookup"><span data-stu-id="aa546-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="aa546-103">Jei kai kuriems vartotojams viešojo aplanko prieiga neveikia, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="aa546-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="aa546-104">Prisijunkite prie "EXO PowerShell" ir Konfigūruokite parametrą DefaultPublicFolderMailbox, esantį probleminiame vartotojo abonemente, kad jis atitiktų vartotojo paskyros parametrą.</span><span class="sxs-lookup"><span data-stu-id="aa546-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="aa546-105">Pavyzdžiui</span><span class="sxs-lookup"><span data-stu-id="aa546-105">Example:</span></span>

<span data-ttu-id="aa546-106">Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="aa546-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="aa546-107">Nustatyti pašto dėžutės probleminių vartotojų – DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="aa546-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="aa546-108">Palaukite bent vieną valandą, kad pakeitimai įsigaliotų.</span><span class="sxs-lookup"><span data-stu-id="aa546-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="aa546-109">Jei problema išlieka, atlikite [šią procedūrą](https://aka.ms/pfcte) , kad išspręstumėte viešojo aplanko prieigos problemas naudodami "Outlook".</span><span class="sxs-lookup"><span data-stu-id="aa546-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="aa546-110">**Norėdami valdyti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami "Outlook"**:</span><span class="sxs-lookup"><span data-stu-id="aa546-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="aa546-111">Naudokite Set-CASMailbox <mailboxname> -publicfolderclientaccess $TRUE arba $FALSE</span><span class="sxs-lookup"><span data-stu-id="aa546-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="aa546-112">$true: leisti vartotojams pasiekti viešuosius aplankus programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="aa546-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="aa546-113">$false: uždrausti vartotojų prieigą prie viešųjų aplankų programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="aa546-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="aa546-114">– tai yra numatytoji reikšmė.</span><span class="sxs-lookup"><span data-stu-id="aa546-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="aa546-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="aa546-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="aa546-116">**Pastaba** Ši procedūra gali valdyti ryšius tik su "Outlook" kompiuteriu, skirtais "Windows" klientams.</span><span class="sxs-lookup"><span data-stu-id="aa546-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="aa546-117">Vartotojas gali toliau naudotis viešaisiais aplankais naudodami OWA arba "Outlook for Mac".</span><span class="sxs-lookup"><span data-stu-id="aa546-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="aa546-118">Daugiau informacijos ieškokite straipsnyje [palaikymo, skirto valdomam ryšiui su viešaisiais aplankais programoje "Outlook", palaikymas](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="aa546-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>