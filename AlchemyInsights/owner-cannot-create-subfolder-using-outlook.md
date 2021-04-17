---
title: Savininkas negali sukurti poaplankių naudodamas "Outlook"
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836143"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Savininkas negali sukurti poaplankių naudodamas "Outlook"

**Nuolat kyla problemų dėl viešųjų aplankų savininkų, kurie kuria poaplankius naudodami "Outlook". Netrukus problema bus išspręsta.**

Tuo tarpu naudokite vieną iš šių sprendimų:

1. "Outlook for MAC" naudojimas norint sukurti poaplankį, nes problema veikia tik "Outlook", skirtą staliniams langams (visos versijos)
2. Administratoriaus sukurti poaplankį naudojant EXO apvalkalą arba EAC
3. "DefaultPublicFolderMailbox" / "EffectivePublicFolderMailbox" keitimas į kitą vartotojo pašto dėžutę, o ne į aplanko turinio pašto dėžutę, dėl kurios kyla problemų  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Palaukite valandą, iš naujo paleiskite "Outlook" klientą