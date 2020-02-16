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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="7d8d4-102">Panaikinto viešojo aplanko atkūrimas</span><span class="sxs-lookup"><span data-stu-id="7d8d4-102">Restore a deleted public folder</span></span>

<span data-ttu-id="7d8d4-103">**Norėdami atkurti panaikintus elementus iš viešojo aplanko**:</span><span class="sxs-lookup"><span data-stu-id="7d8d4-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="7d8d4-104">See [you negali atkurti ištrintus elementus iš ne pašto viešąjį aplanką Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="7d8d4-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="7d8d4-105">**Jei norite atkurti ištrintą viešąjį aplanką (bet kokio tipo)**:</span><span class="sxs-lookup"><span data-stu-id="7d8d4-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="7d8d4-106">Prašome naudoti po EXO PowerShell komandą:</span><span class="sxs-lookup"><span data-stu-id="7d8d4-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="7d8d4-107">Sintaksė:</span><span class="sxs-lookup"><span data-stu-id="7d8d4-107">Syntax:</span></span>

    ><span data-ttu-id="7d8d4-108">$pf = gauti-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Pavadinimas-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. tapatybę-kelio \<maršrutas, kuriame aplankas bus atkurtas></span><span class="sxs-lookup"><span data-stu-id="7d8d4-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="7d8d4-109">Pavyzdys: Ši komanda atkurs Subfolder1 ir pastatys ją \Parent1:</span><span class="sxs-lookup"><span data-stu-id="7d8d4-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="7d8d4-110">$pf = gauti-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Recurse |? {$_. Pavadinimas-EQ "Subfolder1"}; Set-PublicFolder $pf. tapatybė-kelias \ parent1</span><span class="sxs-lookup"><span data-stu-id="7d8d4-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="7d8d4-111">Daugiau informacijos rasite [panaikinto viešojo aplanko atkūrimas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="7d8d4-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
