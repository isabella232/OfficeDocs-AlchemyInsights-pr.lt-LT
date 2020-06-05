---
title: "\"Microsoft 365\" grupės el. pašto adreso keitimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580665"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="b8779-102">"Microsoft 365" grupės el. pašto adreso keitimas</span><span class="sxs-lookup"><span data-stu-id="b8779-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="b8779-103">Galite pakeisti "Microsoft 365" grupės el. pašto adresą naudodami administravimo centrą.</span><span class="sxs-lookup"><span data-stu-id="b8779-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="b8779-104">Tiesiog pasirinkite grupę ir pasirinkite @edit el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="b8779-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="b8779-105">Taip pat galite naudoti šią komandą EXO PowerShell pakeisti pagrindinis SMTP adresas Microsoft 365 grupės:</span><span class="sxs-lookup"><span data-stu-id="b8779-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="b8779-106">Set-UnifiedGroup - PrimarySmtpAddress Nustatyti UnifiedGroup <Group Name> - PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="b8779-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="b8779-107">Pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="b8779-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
