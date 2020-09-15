---
title: Nurodymai, kaip Slėpti/neslėpti grupės adresų sąraše
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
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663017"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>"Microsoft 365" grupės slėpimas iš adresų sąrašo (GAL)

Norėdami slėpti "Microsoft 365" grupę iš "Exchange" klientų adresų sąrašų (GAL) (pvz., "Outlook" arba OWA), naudokite šią komandą "EXO Shell":

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Norėdami slėpti "Microsoft 365" grupę, kad ji būtų matoma "Exchange" klientams, naudokite šią komandą "EXO Shell":

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

