---
title: Keisti griežtą slaptažodžio reikalavimą
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286286"
---
# <a name="change-strong-password-requirement"></a>Keisti sudėtingą slaptažodžio reikalavimą

Pagal numatytuosius nustatymus "Microsoft" reikalauja sudėtingų slaptažodžių. 

Naudodami "PowerShell", galite išjungti sudėtingus slaptažodžius konkretiems vartotojams naudodami šią komandą:<br>
*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Daugiau informacijos apie slaptažodžio strategiją](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kaip prisijungti prie "Office 365" naudojant "PowerShell"](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Daugiau informacijos apie "PowerShell MsolUser" komandas](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Atskiro vartotojo slaptažodžio nustatymas niekada nesibaigia](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
