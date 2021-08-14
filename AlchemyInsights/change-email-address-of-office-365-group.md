---
title: El. pašto adreso keitimas Microsoft 365 grupės
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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930737"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>El. pašto adreso keitimas Microsoft 365 grupės

Naudodami administravimo centrą, galite pakeisti Microsoft 365 grupės el. pašto adresą. Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.

Taip pat galite naudoti exo "PowerShell" komandą, norėdami pakeisti pirminį Microsoft 365 SMTP adresą:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Pavyzdys:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
