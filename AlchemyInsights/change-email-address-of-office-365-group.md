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
# <a name="change-email-address-of-an-microsoft-365-group"></a>"Microsoft 365" grupės el. pašto adreso keitimas

Galite pakeisti "Microsoft 365" grupės el. pašto adresą naudodami administravimo centrą. Tiesiog pasirinkite grupę ir pasirinkite @edit el. pašto adresą.

Taip pat galite naudoti šią komandą EXO PowerShell pakeisti pagrindinis SMTP adresas Microsoft 365 grupės:

Set-UnifiedGroup - PrimarySmtpAddress Nustatyti UnifiedGroup <Group Name> - PrimarySmtpAddress<new SMTP Address>

Pavyzdys:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
