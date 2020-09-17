---
title: Panaikinto viešojo aplanko atkūrimas
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774539"
---
# <a name="restore-a-deleted-public-folder"></a>Panaikinto viešojo aplanko atkūrimas

**Norėdami atkurti panaikintus elementus iš viešojo aplanko**:

- Sužinokite [, ar negalite atkurti panaikintų elementų iš "Outlook 2016" viešojo aplanko ne pašto viešojo aplanko](https://aka.ms/pfrec).
 
**Norėdami atkurti panaikintą viešąjį aplanką (bet kokio tipo)**: 

- Naudokite šią "EXO PowerShell" komandą:

    Sintaksė

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Pavyzdys: toliau pateikta komanda atkurs Subfolder1 ir padėkite ją dalyje \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Daugiau informacijos rasite [panaikinto viešojo aplanko atkūrimas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
