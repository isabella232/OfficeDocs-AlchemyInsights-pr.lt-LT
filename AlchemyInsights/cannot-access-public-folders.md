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
# <a name="outlook-cannot-connect-to-public-folders"></a>"Outlook" negali prisijungti prie viešųjų aplankų

Jei kai kuriems vartotojams viešojo aplanko prieiga neveikia, bandykite atlikti šiuos veiksmus:

Prisijunkite prie "EXO PowerShell" ir Konfigūruokite parametrą DefaultPublicFolderMailbox, esantį probleminiame vartotojo abonemente, kad jis atitiktų vartotojo paskyros parametrą.

Pavyzdžiui

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Nustatyti pašto dėžutės probleminių vartotojų – DefaultPublicFolderMailbox \<value from previous command>

Palaukite bent vieną valandą, kad pakeitimai įsigaliotų.

Jei problema išlieka, atlikite [šią procedūrą](https://aka.ms/pfcte) , kad išspręstumėte viešojo aplanko prieigos problemas naudodami "Outlook".
 
**Norėdami valdyti, kurie vartotojai gali pasiekti viešuosius aplankus naudodami "Outlook"**:

1.  Naudokite Set-CASMailbox <mailboxname> -publicfolderclientaccess $TRUE arba $FALSE  
      
    $true: leisti vartotojams pasiekti viešuosius aplankus programoje "Outlook"  
      
    $false: uždrausti vartotojų prieigą prie viešųjų aplankų programoje "Outlook". – tai yra numatytoji reikšmė.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Pastaba** Ši procedūra gali valdyti ryšius tik su "Outlook" kompiuteriu, skirtais "Windows" klientams. Vartotojas gali toliau naudotis viešaisiais aplankais naudodami OWA arba "Outlook for Mac".
 
Daugiau informacijos ieškokite straipsnyje [palaikymo, skirto valdomam ryšiui su viešaisiais aplankais programoje "Outlook", palaikymas](https://aka.ms/controlpf).