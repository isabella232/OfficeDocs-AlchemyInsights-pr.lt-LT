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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810492"
---
# <a name="issues-with-azure-mfa"></a>"Azure" MFA problemos
Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudodami kelių dalių autentifikavimą (MFA)

1. Paveiktas vartotojas gali būti užblokuotas "Azure Active Directory" portale. Tokiu atveju autentifikavimo bandymai tam konkrečiam vartotojui bus automatiškai atmesti. [Atlikite šiame straipsnyje nurodytus veiksmus, kad atblokuokite juos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jei vartotojo blokavimas nepadės arba vartotojas nėra užblokuotas, galite pabandyti iš naujo nustatyti vartotojo MFA ir jis vėl pereis per registracijos procesą. [Atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jei pirmą kartą įgalinote MFA ir jūsų vartotojai negali prisijungti prie ne naršyklių klientų, pvz., "Outlook", "Skype" ir kt., galbūt "ADAL" ("Active Directory" autentifikavimo biblioteka) neįgalinta jūsų "O365" prenumeratoje. Tokiu atveju turėsite prisijungti prie "Exchange Online PowerShell" ir paleisti šią "cmdlet":  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*