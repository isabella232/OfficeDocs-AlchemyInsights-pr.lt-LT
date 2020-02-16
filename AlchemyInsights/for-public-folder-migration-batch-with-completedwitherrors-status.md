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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043603"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Viešųjų aplankų perkėlimo paketą su CompletedWithErrors būsena

Atlikite šiuos veiksmus, Norėdami užbaigti partiją, praleidžiant didelius/blogus elementus: 
1. "Perkėlimo" paketo praleista elementų tvirtinimas:

    Set-MigrationBatch \<batchname> Tvirtinveskippeditems 
2. Naudokite šią komandą, kad patvirtintumėte praleistą elementus perkėlimo užklausoms, kurios yra sinchronizuotos, bet neatliktos:

    $pf = gauti-PublicFolderMailboxMigrationRequest | Gauti-PublicFolderMailboxMigrationRequestStatistics-Įskaitymasuosto; ForEach ($i $pf) {jei ($i. Largeitemssusidūrė-gt 0-arba $i. Baditemsaptiko-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}
3. Perkėlimo paketą ir prašymai turėtų atnaujinti ir užbaigti per kelias minutes.

