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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706569"
---
# <a name="change-strong-password-requirement"></a>Keisti sudėtingą slaptažodžio reikalavimą

Pagal numatytuosius nustatymus "Microsoft" reikalauja sudėtingų slaptažodžių. 

Naudodami "PowerShell", galite išjungti sudėtingus slaptažodžius konkretiems vartotojams naudodami šią komandą:<br>
*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Daugiau informacijos apie slaptažodžio strategiją](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kaip prisijungti prie "Microsoft 365" naudojant "PowerShell"](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Daugiau informacijos apie "PowerShell MsolUser" komandas](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
