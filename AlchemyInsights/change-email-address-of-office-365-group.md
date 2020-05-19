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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282928"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="c02c6-102">"Microsoft 365" grupės el. pašto adreso keitimas</span><span class="sxs-lookup"><span data-stu-id="c02c6-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="c02c6-103">Galite pakeisti "Microsoft 365" grupės el. pašto adresą naudodami administravimo centrą.</span><span class="sxs-lookup"><span data-stu-id="c02c6-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c02c6-104">Tiesiog pasirinkite grupę ir pasirinkite @edit el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="c02c6-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c02c6-105">Taip pat galite naudoti šią komandą EXO PowerShell pakeisti pagrindinis SMTP adresas Microsoft 365 grupės:</span><span class="sxs-lookup"><span data-stu-id="c02c6-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="c02c6-106">Set-UnifiedGroup - PrimarySmtpAddress Nustatyti UnifiedGroup <Group Name> - PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c02c6-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c02c6-107">Pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="c02c6-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
