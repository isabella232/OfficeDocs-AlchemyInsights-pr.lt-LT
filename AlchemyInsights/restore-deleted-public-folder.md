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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943383"
---
# <a name="restore-a-deleted-public-folder"></a>Panaikintų viešųjų aplankų atkūrimas

**Norėdami atkurti panaikintus elementus iš viešojo aplanko:**

- Žr. [Negalite atkurti panaikintų elementų iš ne pašto](https://aka.ms/pfrec)viešojo aplanko Outlook 2016 .
 
**Norėdami atkurti panaikintus viešuosius aplankus (bet kokio tipo)**: 

- Naudokite šią EXO "PowerShell" komandą:

    Sintaksė:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Pavyzdys: Ši komanda atkurs poaplankį1 ir įdės jį į \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Daugiau [informacijos žr. Panaikintų viešųjų](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) aplankų atkūrimas.
