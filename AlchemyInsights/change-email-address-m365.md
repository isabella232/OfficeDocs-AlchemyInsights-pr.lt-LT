---
title: „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819088"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>„Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas

Naudojant [„Microsoft 365“ administravimo centrą](https://admin.microsoft.com/) galima pakeisti „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adresą. Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.

Taip pat galima naudoti komandą tolesnę „EXO PowerShell“ komandą, kad būtų galima pakeisti „Microsoft 365“ grupės / „Teams“ pagrindinį SMTP adresą:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Pavyzdys:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
