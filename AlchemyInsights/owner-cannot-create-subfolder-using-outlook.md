---
title: Savininkas negali kurti antrinio aplanko naudodamas "Outlook"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665726"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Savininkas negali kurti antrinio aplanko naudodamas "Outlook"

**Yra vykstanti problema su viešojo aplanko savininkais kuriant poaplankius naudojant "Outlook". Problema bus išspręsta netrukus.**

Tuo tarpu naudokite vieną iš šių sprendimų:

1. Naudokite "Outlook", skirtą "MAC", Norėdami sukurti poaplankį, nes problemos poveikis tik "Outlook", skirtoje staliniams kompiuteriams
2. Ar administratorius sukuria poaplankį naudodamas "EXO Shell" arba EAC
3. Pakeiskite DefaultPublicFolderMailbox/EffectivePublicFolderMailbox vartotojui į kitą pašto dėžutę, nei dėl problemų sukėlusio aplanko turinio pašto dėžutę  
    - *Set-Mailbox 1 vartotojas DefaultPublicFolderMailbox PubMBX3*
4. Palaukite valandą, iš naujo paleiskite "Outlook Client"