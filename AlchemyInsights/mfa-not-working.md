---
title: Problemos su MFP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768845"
---
# <a name="issues-with-azure-mfa"></a>Problemos su Azure MFP
Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudojant kelių dalių autentifikavimas (DTS)

1. Susijusio vartotojo gali būti užblokuotas Azure Active Directory portale. Tokiu atveju autentifikavimas bando, kad konkretus vartotojas bus automatiškai atmestas. [Norėdami atblokuoti, atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jei atblokavimo vartotojas nepadėjo arba vartotojas nėra užblokuotas galite pabandyti iš naujo MFP vartotojo ir jie bus eiti per Registruotis procesas dar kartą. [Atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jei tai pirmas kartas, kai įjungėte DTS ir jūsų vartotojai negali prisijungti prie ne naršyklės klientams, pvz., "Outlook", "Skype" ir tt, galbūt Alma (Active Directory autentifikavimo biblioteka) neįgalintas jūsų O365 prenumeratą. Tokiu atveju jums reikės prisijungti prie Exchange Online "PowerShell" ir paleisti šį cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*