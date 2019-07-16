---
title: Pakeisti sudėtingą slaptažodį reikalavimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701591"
---
# <a name="change-strong-password-requirement"></a>Pakeisti sudėtingą slaptažodį reikalavimas

Sudėtingus slaptažodžius reikia pagal numatytuosius nustatymus. 

Naudodami "PowerShell" galite išjungti sudėtingus slaptažodžius konkretiems vartotojams su šią komandą:<br>
*Rinkinys-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Daugiau informacijos apie slaptažodžių strategija](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kaip prisijungti prie O365 su "PowerShell"](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Daugiau informacijos apie PowerShell MsolUser komandos](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)