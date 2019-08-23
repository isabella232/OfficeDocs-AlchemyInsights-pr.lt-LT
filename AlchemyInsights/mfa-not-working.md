---
title: Problemas, susijusias su URM
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545181"
---
# <a name="issues-with-mfa"></a>Problemas, susijusias su URM
Yra keletas dalykų, kuriuos reikia patikrinti, jei vartotojai negali prisijungti naudodami kelių dalių autentifikavimas (DTS)

1. Įtakos vartotojas gali būti blokuojami Azure Active Directory portale. Jei tai byla, autentifikavimo bandymų, kad konkrečiam vartotojui bus automatiškai atmesti. [Atlikite veiksmus šiame straipsnyje, atblokuoti juos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jei vartotojo atblokavimas nepadėjo arba vartotojas nėra užblokuota galite bandyti iš naujo URM vartotojas ir jie bus eiti per Registruotis procesą dar kartą. [Atlikite veiksmus šiame straipsnyje.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jei tai pirmas kartas, tu įgalintas MFP ir vartotojams negalite prisijungti prie naršyklės Klientai pvz., "Outlook", "Skype" ir t.t., gal Alma (Active Directory autentifikavimo bibliotekos) nėra įjungtas prenumeratą O365. Tokiu atveju jums reikės prisijungti prie Exchange Online "PowerShell" ir vykdyti šį cmdlet:  *Set-OrganizationalSetting-OAuth2ClientProfileEnabled: $true*