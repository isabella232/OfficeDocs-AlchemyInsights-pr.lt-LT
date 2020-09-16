---
title: Viešojo aplanko perkėlimo paketui su CompletedWithErrors būsena
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744121"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Viešojo aplanko perkėlimo paketui su CompletedWithErrors būsena

Atlikite toliau nurodytus veiksmus, kad užbaigtumėte paketą, praleidžiamas didžiulis/blogas elementas: 
1. Patvirtinti praleistus elementus perkėlimo pakete:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Naudokite šią komandą Norėdami patvirtinti praleistus elementus perkėlimo užklausose, kurios yra "sinchronizuotos", tačiau neatliktos:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Perkėlimo paketas ir prašymai turėtų būti atnaujinti ir baigti per kelias minutes.

