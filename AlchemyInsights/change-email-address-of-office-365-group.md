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
# <a name="change-email-address-of-a-microsoft-365-group"></a>"Microsoft 365" grupės el. pašto adreso keitimas

Galite pakeisti "Microsoft 365" grupės el. pašto adresą naudodami administravimo centrą. Tiesiog pasirinkite grupę ir pasirinkite @edit el. pašto adresą.

Taip pat galite naudoti šią komandą EXO PowerShell pakeisti pagrindinis SMTP adresas Microsoft 365 grupės:

Set-UnifiedGroup - PrimarySmtpAddress Nustatyti UnifiedGroup <Group Name> - PrimarySmtpAddress<new SMTP Address>

Pavyzdys:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
