---
title: Savininkas negali sukurti poaplankio naudodamas "Outlook"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749138"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Savininkas negali sukurti poaplankio naudodamas "Outlook"

**Yra problema su viešųjų aplankų savininkai sukurti poaplankius naudojant "Outlook". Problema bus išspręsta netrukus.**

Tuo tarpu, naudokite vieną iš šių sprendimų:

1. Naudokite "Outlook", skirta MAC sukurti poaplankį, kaip problema turi įtakos tik "Outlook", skirta darbalaukio windows (visos versijos)
2. Ar administratorius sukurti poaplankį naudojant EXO Shell arba EAC
3. Pakeisti DefaultPublicFolderMailbox/EffectivePublicFolderMailbox vartotojo į kitą pašto dėžutę nei turinio pašto dėžutės aplanko sukelia problema  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Palaukite valandą, iš naujo paleiskite "Outlook" kliento