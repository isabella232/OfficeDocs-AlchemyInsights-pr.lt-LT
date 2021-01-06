---
title: „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756565"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>„Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas

Naudojant [„Microsoft 365“ administravimo centrą](https://admin.microsoft.com/) galima pakeisti „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adresą. Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.

Taip pat galima naudoti komandą tolesnę „EXO PowerShell“ komandą, kad būtų galima pakeisti „Microsoft 365“ grupės / „Teams“ pagrindinį SMTP adresą:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Pavyzdys:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
