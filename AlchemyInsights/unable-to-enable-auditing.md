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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="78712-102">Negalima įgalinti vieningosios tikrinimo</span><span class="sxs-lookup"><span data-stu-id="78712-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="78712-103">Kai bandote įgalinti bendrą organizacijos auditą, galite gauti klaidos pranešimą, panašų į šį:</span><span class="sxs-lookup"><span data-stu-id="78712-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="78712-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="78712-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="78712-105">[Prisijungimas prie "Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)" "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="78712-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="78712-106">Vykdykite šią "cmdlet":</span><span class="sxs-lookup"><span data-stu-id="78712-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="78712-107">Palaukite, kol "60" minutės, kad įsigaliotų ankstesnis parametras.</span><span class="sxs-lookup"><span data-stu-id="78712-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="78712-108">Vykdykite šią komandą "Exchange Online PowerShell":</span><span class="sxs-lookup"><span data-stu-id="78712-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="78712-109">Papildomos informacijos ieškokite šiuose straipsniuose:</span><span class="sxs-lookup"><span data-stu-id="78712-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="78712-110">Prisijungimas prie "Exchange Online" "PowerShell" naudojant kelių dalių autentifikavimą</span><span class="sxs-lookup"><span data-stu-id="78712-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="78712-111">Audito žurnalų ieškos įjungimas arba išjungimas</span><span class="sxs-lookup"><span data-stu-id="78712-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
