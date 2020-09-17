---
title: Negalima pasiekti viešųjų aplankų
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812555"
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