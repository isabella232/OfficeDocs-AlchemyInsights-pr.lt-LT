---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007798"
---
# <a name="unable-to-enable-unified-auditing"></a>Nepavyko įgalinti vieningojo audito

Kai bandote įgalinti bendrą organizacijos auditą, galite gauti klaidos pranešimą, panašų į šį:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:

1. [Prisijungimas "Exchange Online PowerShell".](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Vykdykite šią "cmdlet":

   ```
   Enable-OrganizationCustomization
   ```

3. Palaukite 60 minučių, kol įsigalios ankstesnis parametras.

4. Vykdykite šią "PowerShell" Exchange Online komandą:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Daugiau informacijos žr. šiuos straipsnius:

- [Prisijungimas"Exchange Online"PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Audito žurnalo ieškos įjungimas arba išjungimas](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
