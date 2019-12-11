---
title: Negalite prieiti prie viešųjų aplankų
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959502"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>"Outlook" negali prisijungti prie viešųjų aplankų

Jei prieiga prie viešojo aplanko neveikia keliems vartotojams, išbandykite toliau nurodytus veiksmus.

Prisijungti prie EXO PowerShell ir sukonfigūruoti DefaultPublicFolderMailbox problema vartotojo abonementą, kad atitiktų vieną darbo vartotojo abonementą.

Pavyzdys:

Gauk-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, Poveikivepublicfoldermailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<reikšmę iš ankstesnės komandos>

Palaukite bent vieną valandą, kol pakeitimas įsigalios.