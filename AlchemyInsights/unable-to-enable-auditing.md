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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="f9b75-102">Neįmanoma įgalinti vieningosios audito</span><span class="sxs-lookup"><span data-stu-id="f9b75-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="f9b75-103">Bandant įjungti bendrą audito organizacijoje "Office 365", galite gauti klaidos panaši į šį:</span><span class="sxs-lookup"><span data-stu-id="f9b75-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="f9b75-104">Norėdami išspręsti šią problemą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="f9b75-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="f9b75-105">[Prisijungti prie keistis internete "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="f9b75-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="f9b75-106">Vykdykite šią cmdlet:</span><span class="sxs-lookup"><span data-stu-id="f9b75-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="f9b75-107">Palaukite 60 minučių už ankstesnį parametrui turi įsigalioti.</span><span class="sxs-lookup"><span data-stu-id="f9b75-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="f9b75-108">Vykdykite toliau nurodytą komandą Exchange Online "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="f9b75-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="f9b75-109">Papildomos informacijos ieškokite šiuose straipsniuose:</span><span class="sxs-lookup"><span data-stu-id="f9b75-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="f9b75-110">Prisijungti prie Exchange Online "PowerShell" naudoja kelių dalių autentifikavimas</span><span class="sxs-lookup"><span data-stu-id="f9b75-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="f9b75-111">Įjungti arba išjungti "Office 365" audito žurnalo paieška</span><span class="sxs-lookup"><span data-stu-id="f9b75-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
