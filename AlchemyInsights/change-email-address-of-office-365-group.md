---
title: "\"Microsoft 365\" grupės el. pašto adreso keitimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819052"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>"Microsoft 365" grupės el. pašto adreso keitimas

Galite pakeisti "Microsoft 365" grupės el. pašto adresą naudodami administravimo centrą. Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.

Taip pat galite naudoti exo "PowerShell" komandą norėdami pakeisti pagrindinį "Microsoft 365" grupės SMTP adresą:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Pavyzdys:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
