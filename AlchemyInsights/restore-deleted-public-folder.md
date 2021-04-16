---
title: Panaikintų viešųjų aplankų atkūrimas
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809447"
---
# <a name="restore-a-deleted-public-folder"></a>Panaikintų viešųjų aplankų atkūrimas

**Norėdami atkurti panaikintus elementus iš viešojo aplanko:**

- Žr. [Negalite atkurti panaikintų elementų iš ne pašto viešojo aplanko programoje "Outlook 2016".](https://aka.ms/pfrec)
 
**Norėdami atkurti panaikintus viešuosius aplankus (bet kokio tipo)**: 

- Naudokite šią EXO "PowerShell" komandą:

    Sintaksė:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Pavyzdys: Ši komanda atkurs poaplankį1 ir įdės jį į \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Daugiau [informacijos žr. Panaikintų viešųjų](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) aplankų atkūrimas.
