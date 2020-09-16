---
title: 2419 – neįmanoma įgalinti – tikrinimas
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767607"
---
# <a name="unable-to-enable-unified-auditing"></a>Negalima įgalinti vieningosios tikrinimo

Kai bandote įgalinti bendrą organizacijos auditą, galite gauti klaidos pranešimą, panašų į šį:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:

1. [Prisijungimas prie "Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)" "PowerShell".

2. Vykdykite šią "cmdlet":

   ```
   Enable-OrganizationCustomization
   ```

3. Palaukite, kol "60" minutės, kad įsigaliotų ankstesnis parametras.

4. Vykdykite šią komandą "Exchange Online PowerShell":

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Papildomos informacijos ieškokite šiuose straipsniuose:

- [Prisijungimas prie "Exchange Online" "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Audito žurnalų ieškos įjungimas arba išjungimas](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
