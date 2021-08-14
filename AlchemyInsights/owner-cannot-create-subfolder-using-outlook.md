---
title: Savininkas negali sukurti poaplankių naudodamas Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063132"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Savininkas negali sukurti poaplankių naudodamas Outlook

**Nuolat kyla problemų dėl viešųjų aplankų savininkų, kurie kuria poaplankius naudodami Outlook. Netrukus problema bus išspręsta.**

Tuo tarpu naudokite vieną iš šių sprendimų:

1. Naudokite "Outlook for MAC", kad sukurtumėte poaplankį, nes problema veikia tik Outlook langus (visas versijas)
2. Administratoriaus sukurti poaplankį naudojant EXO apvalkalą arba EAC
3. "DefaultPublicFolderMailbox" / "EffectivePublicFolderMailbox" keitimas į kitą vartotojo pašto dėžutę, o ne į aplanko turinio pašto dėžutę, dėl kurios kyla problemų  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Palaukite valandą, iš naujo paleiskite "Outlook" klientą