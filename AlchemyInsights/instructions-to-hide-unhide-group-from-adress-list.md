---
title: Instrukcijos slėpti/ rodyti grupę iš adresų sąrašo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908352"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Slėpti "Microsoft 365" grupę iš adresų sąrašo (GAL)

Norėdami paslėpti "Microsoft 365" grupę iš "Exchange" klientų (pvz., "Outlook" arba OWA) adresų sąrašų (GAL), exo apvalkale naudokite šią komandą:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Norėdami paslėpti "Microsoft 365" grupės matomas Exchange klientams, naudokite šią komandą EXO apvalkale:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

