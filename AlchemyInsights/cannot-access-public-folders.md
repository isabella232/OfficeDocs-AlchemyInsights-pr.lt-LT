---
title: Nepavyksta pasiekti viešųjų aplankų
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891757"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Programa Outlook negali prisijungti prie viešųjų aplankų

Jei kai kuriems vartotojams viešojo aplanko prieiga neveikia, pabandykite atlikti šiuos veiksmus:

Prisijunkite prie EXO "PowerShell" ir sukonfigūruokite parametrą DefaultPublicFolderMailbox problemos vartotojo abonemente, kad atitiktų parametrą, esantį veikiančiame vartotojo abonemente.

Pavyzdys:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox ft Default

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<reikšmė iš ankstesnės komandos>

Palaukite bent vieną valandą, kol pakeitimas įsigalios.

Jei problema išlieka, atlikite [šią procedūrą,](https://aka.ms/pfcte) norėdami išspręsti viešųjų aplankų prieigos problemas naudodami "Outlook".