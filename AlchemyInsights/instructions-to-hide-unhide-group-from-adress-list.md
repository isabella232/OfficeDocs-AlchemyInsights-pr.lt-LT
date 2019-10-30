---
title: Instrukcijos paslėpti/Neslėpti grupę iš adresų sąrašo
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768936"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Slėpti Office 365 grupę iš adresų sąrašo (GAL)

Norėdami paslėpti "Office 365" grupę iš adresų sąrašų (GAL) Exchange klientų (pvz., "Outlook" arba OWA), naudokite šią komandą EXO apvalkalas:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Norėdami paslėpti Office 365 grupė yra matomas Exchange klientams, naudokite šią komandą EXO apvalkalas:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

