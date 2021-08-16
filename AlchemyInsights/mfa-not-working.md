---
title: MFA problemos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098610"
---
# <a name="issues-with-azure-mfa"></a>"Azure" MFA problemos
Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudodami kelių dalių autentifikavimą (MFA)

1. Paveiktas vartotojas gali būti užblokuotas "Azure Active Directory" portale. Tokiu atveju autentifikavimo bandymai tam konkrečiam vartotojui bus automatiškai atmesti. [Atlikite šiame straipsnyje nurodytus veiksmus, kad atblokuokite juos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jei vartotojo blokavimas nepadės arba vartotojas nėra užblokuotas, galite pabandyti iš naujo nustatyti vartotojo MFA ir jis vėl pereis per registracijos procesą. [Atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jei pirmą kartą įgalinote MFA ir jūsų vartotojai negali prisijungti prie ne naršyklių klientų, pvz., "Outlook", "Skype" ir kt., galbūt "ADAL" ("Active Directory" autentifikavimo biblioteka) neįgalinta jūsų "O365" prenumeratoje. Tokiu atveju turėsite prisijungti prie "Exchange Online PowerShell" ir paleisti šią "cmdlet": *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*