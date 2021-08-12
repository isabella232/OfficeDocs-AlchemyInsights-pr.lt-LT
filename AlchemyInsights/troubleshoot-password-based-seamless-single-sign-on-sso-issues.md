---
title: Slaptažodžiu pagrįstos sklandžiosios bendrosios a prisijungimo (SSO) trikčių šalinimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972832"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Slaptažodžiu pagrįstos sklandžiosios bendrosios a prisijungimo (SSO) trikčių šalinimas

Norėdami sužinoti slaptažodžiu pagrįsto SSO pagrindu sukurtus pagrindus, žr. [Slaptažodžiu pagrįstas autentifikavimas naudojant "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Slaptažodžiu pagrįsto SSO konfigūravimas**

1. [Sukonfigūruokite slaptažodžiu pagrįstą bendrąją](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) adresą – šiame straipsnyje pateikiama daugiau informacijos apie slaptažodžiu pagrįstą SSO parinktį. Jei jūsų pridedamai programai reikia pasirinktinės konfigūracijos ir turite naudoti slaptažodžiu pagrįstą SSO, šis straipsnis skirtas jums.
2. [Sukonfigūruokite slaptažodžiu pagrįstą](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) bendrąją ženklą, kad būtų galima naudoti "on-prem" programas – taikomosios programos tarpinis serveris palaiko kelis bendrosios a prisijungimo režimus. Slaptažodžiu pagrįstas prisijungimas skirtas programoms, kurios autentifikavimui naudoja vartotojo vardo / slaptažodžio derinį. Kai konfigūruojate savo taikomosios programos slaptažodžiu pagrįstą adresą, vartotojai turi vieną kartą prisijungti prie vietinės taikomosios programos. Po to "Azure Active Directory" prisijungimo informaciją ir automatiškai pateikia ją programai, kai jūsų vartotojai ją pasieks nuotoliniu būdu.
    - Jau turėjote publikuoti ir išbandyti savo programą naudodami programos tarpinį serverį. Jei ne, atlikite veiksmus, nurodytus Taikomųjų programų publikavimas naudojant ["Azure AD"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) taikomosios programos tarpinį serverį, tada tęskite slaptažodžiu pagrįstos SSO konfigūravimą dėl "on-prem" programų.

Norėdami šalinti slaptažodžiu pagrįstos SSO triktis, žr. [Slaptažodžiais pagrįstos bendrosios a prisijungimo trikčių šalinimas naudojant "Azure AD"](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
