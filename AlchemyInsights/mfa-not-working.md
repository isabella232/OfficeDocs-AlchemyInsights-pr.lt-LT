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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545181"
---
# <a name="issues-with-mfa"></a>Problemos su MFP
Yra keletas dalykų, kuriuos reikia patikrinti, ar vartotojai negali prisijungti naudojant kelių dalių autentifikavimas (DTS)

1. Susijusio vartotojo gali būti užblokuotas Azure Active Directory portale. Tokiu atveju autentifikavimas bando, kad konkretus vartotojas bus automatiškai atmestas. [Norėdami atblokuoti, atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jei atblokavimo vartotojas nepadėjo arba vartotojas nėra užblokuotas galite pabandyti iš naujo MFP vartotojo ir jie bus eiti per Registruotis procesas dar kartą. [Atlikite šiame straipsnyje nurodytus veiksmus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jei tai pirmas kartas, kai įjungėte DTS ir jūsų vartotojai negali prisijungti prie ne naršyklės klientams, pvz., "Outlook", "Skype" ir tt, galbūt Alma (Active Directory autentifikavimo biblioteka) neįgalintas jūsų O365 prenumeratą. Tokiu atveju jums reikės prisijungti prie Exchange Online "PowerShell" ir paleisti šį cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*