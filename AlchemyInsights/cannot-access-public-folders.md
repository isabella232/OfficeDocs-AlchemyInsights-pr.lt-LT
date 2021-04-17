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
# <a name="outlook-cannot-connect-to-public-folders"></a>"Outlook" negali prisijungti prie viešųjų aplankų

Jei viešojo aplanko prieiga neveikia kai kuriems vartotojams, pabandykite atlikti šiuos veiksmus:

Prisijunkite prie EXO "PowerShell" ir sukonfigūruokite parametrą DefaultPublicFolderMailbox problemos vartotojo paskyroje, kad jis atitiktų darbingo vartotojo paskyros parametrą.

Pavyzdys:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemaUser -DefaultPublicFolderMailbox \<value from previous command>

Palaukite bent vieną valandą, kol pakeitimas įsigalios.

Jei problema išlieka, atlikite šią procedūrą ir [pašalinkite viešojo](https://aka.ms/pfcte) aplanko prieigos problemas naudodami "Outlook".
 
**Norėdami kontroliuoti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami "Outlook":**

1.  <mailboxname>"Set-CASMailbox-PublicFolderClientAccess" $true arba "$false  
      
    $true: leisti vartotojams pasiekti viešuosius aplankus programoje "Outlook"  
      
    $false: neleisti vartotojams pasiekti viešųjų aplankų programoje "Outlook". – tai yra numatytoji reikšmė.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Pastaba** Ši procedūra gali valdyti ryšius tik su "Outlook" darbalaukiu, skirta "Windows" klientams. Vartotojas gali toliau pasiekti viešuosius aplankus naudodamas OWA arba "Outlook", skirtą "Mac".
 
Daugiau informacijos žr. ["Outlook" valdomi ryšiai su viešais aplankais valdomi palaikymo paskelbimas.](https://aka.ms/controlpf)