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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="bb325-102">„Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas</span><span class="sxs-lookup"><span data-stu-id="bb325-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="bb325-103">Naudojant [„Microsoft 365“ administravimo centrą](https://admin.microsoft.com/) galima pakeisti „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="bb325-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="bb325-104">Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="bb325-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="bb325-105">Taip pat galima naudoti komandą tolesnę „EXO PowerShell“ komandą, kad būtų galima pakeisti „Microsoft 365“ grupės / „Teams“ pagrindinį SMTP adresą:</span><span class="sxs-lookup"><span data-stu-id="bb325-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="bb325-106">Pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="bb325-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
