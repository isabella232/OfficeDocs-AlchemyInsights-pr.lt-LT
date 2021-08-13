---
title: Grupės slėpimo / slėpimo iš adresų sąrašo instrukcijos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926253"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Slėpti Microsoft 365 grupę iš adresų sąrašo (GAL)

Norėdami paslėpti Microsoft 365 grupę iš "Exchange" klientų adresų sąrašų (GAL) (pvz., "Outlook" arba "OWA"), naudokite šią komandą EXO aplinkoje:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Norėdami paslėpti Microsoft 365 grupę, kad ji nebūtų matoma Exchange klientams, naudokite šią komandą EXO aplinkoje:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

