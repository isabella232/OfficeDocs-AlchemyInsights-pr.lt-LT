---
title: Nepagrįstų vienkartinio prisijungimo (SSO) problemų sprendimas slaptažodžiu
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714880"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Nepagrįstų vienkartinio prisijungimo (SSO) problemų sprendimas slaptažodžiu

Jei norite sužinoti, kas yra "SSO" slaptažodį, ieškokite [slaptažodžiu pagrįstas autentifikavimas naudojant "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)".

**SSO pagal slaptažodį konfigūravimas**

1. [Slaptažodžiu pagrįsto vienkartinio prisijungimo konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – šiame straipsnyje išsamiau apie slaptažodžiu pagrįstą SSO parinktį. Jei įtrauktai taikomajai programai reikia pasirinktinio konfigūravimo ir turite naudoti SSO pagal slaptažodį, tada šis straipsnis skirtas jums.
2. [Slaptažodžiu pagrįsto vienkartinio prisijungimo prie "Prem" taikomųjų programų konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – taikomosios programos tarpinis serveris palaiko kelis bendrosios autentifikacijos režimus. Slaptažodžiu pagrįstas prisijungimas skirtas taikomosioms programoms, kurios naudoja vartotojo vardo ir slaptažodžio derinį autentifikavimui. Sukonfigūravus slaptažodžiu pagrįstą prisijungimo paraišką, vartotojai turi prisijungti prie vietinio taikomosios programos. Po to, "Azure Active Directory" saugo prisijungimo informaciją ir automatiškai pateikia ją taikomajai programai, kai vartotojai ją pasiekia nuotoliniu būdu.
    - Jūs jau turite publikuoti ir išbandyti programą naudodami taikomosios programos tarpinį serverį. Jei ne, atlikite veiksmus [publikuojant taikomąsias programas naudodami "AZURE AD" taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , tada toliau konfigūravimą pagal slaptažodžiu pagrįstą SSO programas.

Jei norite šalinti SSO pagal slaptažodį, žiūrėkite " [Azure AD" bendrosios autentifikacijos "Azure AD" trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
