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
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="8d9de-102">„Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adreso keitimas</span><span class="sxs-lookup"><span data-stu-id="8d9de-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="8d9de-103">Naudojant [„Microsoft 365“ administravimo centrą](https://admin.microsoft.com/) galima pakeisti „Microsoft 365“ grupės arba „Microsoft Teams“ el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="8d9de-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="8d9de-104">Tiesiog pasirinkite grupę ir pasirinkite @redaguoti el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="8d9de-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="8d9de-105">Taip pat galima naudoti komandą tolesnę „EXO PowerShell“ komandą, kad būtų galima pakeisti „Microsoft 365“ grupės / „Teams“ pagrindinį SMTP adresą:</span><span class="sxs-lookup"><span data-stu-id="8d9de-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="8d9de-106">Pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="8d9de-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
