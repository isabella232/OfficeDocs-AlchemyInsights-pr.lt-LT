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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996638"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook negalima prisijungti prie viešųjų aplankų

Jei viešojo aplanko prieiga neveikia kai kuriems vartotojams, pabandykite atlikti šiuos veiksmus:

Prisijungimas "EXO PowerShell" ir sukonfigūruokite parametrą DefaultPublicFolderMailbox problemos vartotojo paskyroje, kad jis atitiktų darbingo vartotojo paskyros parametrą.

Pavyzdys:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemaUser -DefaultPublicFolderMailbox \<value from previous command>

Palaukite bent vieną valandą, kol pakeitimas įsigalios.

Jei problema išlieka, atlikite šią procedūrą, [kad šalinkite](https://aka.ms/pfcte) viešojo aplanko prieigos problemas naudodami Outlook.
 
**Norėdami kontroliuoti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami Outlook:**

1.  <mailboxname>"Set-CASMailbox-PublicFolderClientAccess" $true arba "$false  
      
    $true: leisti vartotojams pasiekti viešuosius aplankus Outlook  
      
    $false: neleisti vartotojui pasiekti viešųjų aplankų Outlook. – tai yra numatytoji reikšmė.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Pastaba** Ši procedūra gali valdyti ryšius tik su "Outlook", skirtais Windows klientams. Vartotojas gali toliau pasiekti viešuosius aplankus naudodamas "OWA" arba "Outlook", skirtą "Mac".
 
Daugiau informacijos žr. "Outlook" paskelbimas Apie valdomą ryšių [su viešais aplankais palaikymą.](https://aka.ms/controlpf)