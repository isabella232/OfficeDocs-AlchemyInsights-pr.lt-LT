---
title: 2419-nepavyko atlikti įgalinančios audito
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510436"
---
# <a name="unable-to-enable-unified-auditing"></a>Neįmanoma įgalinti vieningo tikrinimo

Kai bandote įgalinti vieningą auditą savo organizacijoje, galite gauti klaidos pranešimą, panašų į šį:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:

1. [Prisijunkite prie "Exchange Online PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Vykdykite šią cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Palaukite 60 minučių, kol įsigalios ankstesnis parametras.

4. Vykdykite šią komandą Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Jei norite gauti papildomos informacijos, ieškokite šiuose straipsniuose:

- [Prisijungimas prie "Exchange Online PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Audito žurnalo ieškos įjungimas arba išjungimas](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
