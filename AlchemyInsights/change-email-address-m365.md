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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995630"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>„Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas

Naudojant [„Microsoft 365“ administravimo centrą](https://admin.microsoft.com/) galima pakeisti „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adresą. Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.

Taip pat galima naudoti komandą tolesnę „EXO PowerShell“ komandą, kad būtų galima pakeisti „Microsoft 365“ grupės / „Teams“ pagrindinį SMTP adresą:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Pavyzdys:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
