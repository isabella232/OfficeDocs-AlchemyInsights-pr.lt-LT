---
title: Panaikinto viešojo aplanko atkūrimas
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063700"
---
# <a name="restore-a-deleted-public-folder"></a>Panaikinto viešojo aplanko atkūrimas

**Norėdami atkurti panaikintus elementus iš viešojo aplanko**:

- See [you negali atkurti ištrintus elementus iš ne pašto viešąjį aplanką Outlook 2016](https://aka.ms/pfrec).
 
**Jei norite atkurti ištrintą viešąjį aplanką (bet kokio tipo)**: 

- Prašome naudoti po EXO PowerShell komandą:

    Sintaksė:

    >$pf = gauti-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Pavadinimas-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. tapatybę-kelio \<maršrutas, kuriame aplankas bus atkurtas>

    Pavyzdys: Ši komanda atkurs Subfolder1 ir pastatys ją \Parent1:

    >$pf = gauti-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Pavadinimas-EQ "Subfolder1"}; Set-PublicFolder $pf. tapatybė-kelias \ parent1

Daugiau informacijos rasite [panaikinto viešojo aplanko atkūrimas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
