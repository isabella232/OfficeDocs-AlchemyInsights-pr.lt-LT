---
title: Viešųjų aplankų perkėlimo paketą su CompletedWithErrors būsena
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158622"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Viešųjų aplankų perkėlimo paketą su CompletedWithErrors būsena

Atlikite šiuos veiksmus, Norėdami užbaigti partiją, praleidžiant didelius/blogus elementus: 
1. "Perkėlimo" paketo praleista elementų tvirtinimas:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Naudokite šią komandą, kad patvirtintumėte praleistą elementus perkėlimo užklausoms, kurios yra sinchronizuotos, bet neatliktos:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Perkėlimo paketą ir prašymai turėtų atnaujinti ir užbaigti per kelias minutes.

