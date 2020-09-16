---
title: "\"MFA\" problemos"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755139"
---
# <a name="issues-with-azure-mfa"></a>"Azure MFA" problemos
Yra keletas dalykų, kuriuos galite patikrinti, jei vartotojai negali prisiregistruoti naudodami kelių dalių autentifikavimą (MFA)

1. Paveiktą vartotoją galima užblokuoti "Azure Active Directory" portale. Jei tai yra atvejis, konkretaus vartotojo autentifikavimo bandymai bus automatiškai atmesti. [Norėdami atblokuoti, atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jei vartotojui neužblokuotas vartotojas arba vartotojas neužblokuotas, galite pabandyti iš naujo nustatyti vartotojo MFA ir jie pereis į registruotis procesą dar kartą. [Atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jei MFA įgalino pirmą kartą ir jūsų vartotojai negali prisijungti prie naršyklių ne naršyklės, pvz., "Outlook", "Skype" ir kt., galbūt "ADAL" ("Active Directory" autentifikavimo biblioteka) neįgalinta jūsų "O365" prenumeratoje. Šiuo atveju jums reikės prisijungti prie "Exchange Online" "PowerShell" ir paleisti šį "cmdlet":  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*