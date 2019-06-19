---
title: 2419-negali-į-įgalinti-auditas
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065673"
---
# <a name="unable-to-enable-unified-auditing"></a>Neįmanoma įgalinti vieningosios audito

Bandant įjungti bendrą audito organizacijoje "Office 365", galite gauti klaidos panaši į šį:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:

1. [Prisijungti prie keistis internete "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Vykdykite šią cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Palaukite 60 minučių už ankstesnį parametrui turi įsigalioti.

4. Vykdykite toliau nurodytą komandą Exchange Online "PowerShell".

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Papildomos informacijos ieškokite šiuose straipsniuose:

- [Prisijungti prie Exchange Online "PowerShell" naudoja kelių dalių autentifikavimas](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Įjungti arba išjungti "Office 365" audito žurnalo paieška](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
