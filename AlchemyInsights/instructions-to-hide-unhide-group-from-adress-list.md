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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580017"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Slėpti "Microsoft 365" grupę iš adresų sąrašo (GAL)

Norėdami paslėpti "Microsoft 365" grupę iš "Exchange" klientų (pvz., "Outlook" arba OWA) adresų sąrašų (GAL), exo apvalkale naudokite šią komandą:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Norėdami paslėpti "Microsoft 365" grupės matomas Exchange klientams, naudokite šią komandą EXO apvalkale:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

