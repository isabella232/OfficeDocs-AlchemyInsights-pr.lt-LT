---
title: Grupių arba komandų slėpimas arba Office 365 iš adresų sąrašo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088404"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Grupių arba komandų slėpimas arba Office 365 iš adresų sąrašo

Naudokite šią EXO "PowerShell" komandą, kad paslėptumėte arba atžymėtumėte Office 365 / komandas iš "Exchange" klientų (Outlook, OWA) adresų sąrašų (GAL):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Naudokite šią EXO "PowerShell" komandą, kad paslėptumėte arba atžymėtumėte "Office365" grupę / komandas iš "Exchange" klientų (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Išsamias instrukcijas [žr. Office 365 grupių slėpimas iš GAL ir Exchange klientų](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
