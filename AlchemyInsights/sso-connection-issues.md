---
title: SSO prisijungimo problemos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935153"
---
# <a name="sso-connection-issues"></a>SSO prisijungimo problemos

1. Vadovaukitės " [QuickStart": konfigūruokite taikomųjų programų vadovo ypatybes](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) , kad konfigūruotumėte taikomąją programą.
2. Atsižvelgdami į pasirinktą programos ir [bendrosios autentifikacijos parinktį](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) , vadovaukitės toliau pateikiamais nurodymais:
    - Jei norite sukonfigūruoti **vietinę taikomąją programą** , **pagrįstą vienkartiniam autentifikacija**, skaitykite ["SAML" vienkartinio prisijungimo, skirto vietinėms programoms, naudojant taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Norėdami sukonfigūruoti **debesies taikomąją programą** , skirtą **vienkartiniam autentifikacija**, skaitykite  [bendrosios autentifikacijos konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Norėdami sukonfigūruoti **vietinę taikomąją** programą, skirtą **vienkartiniam autentifikacija naudojant taikomosios programos tarpinį serverį**, peržiūrėkite [bendrosios autentifikacijos slaptažodį naudojant taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Taikomųjų programų tarpinio serverio problemų trikčių diagnostika**: rekomenduojame pradėti peržiūrėti trikčių šalinimo srautą, [derinti taikomosios programos tarpinio serverio jungties problemas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), kad nustatytumėte, ar taikomosios programos tarpinio serverio jungtys tinkamai sukonfigūruotos. Jei vis dar kyla problemų jungiantis prie taikomosios programos, vykdykite trikčių šalinimo srauto taikomosios programos [tarpinio serverio taikomosios programos problemas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). " [CORS" problemas galite identifikuoti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) naudodami naršyklės derinimo įrankius:
    - Paleisk naršyklę ir naršykite į žiniatinklio programą.
    - Paspauskite **F12** , kad iškviestumėte derinimo konsolę.
    - Pabandykite atkurti operaciją ir peržiūrėkite konsolės pranešimą. CORS pažeidimas sukuria konsolės klaidą apie kilmę.
    - Kai kurios "CORS" problemos neišsprendžiamos, pvz., kai jūsų programa nukreipia į "login.microsoft.com" ir "Access" atpažinimo ženklo galiojimo laikas baigsis. Tada nepavyksta. Šio scenarijaus sprendimo būdas – pratęsti "Access" atpažinimo ženklo galiojimo laiką, kad jis nesibaigtų vartotojo seanso metu. Daugiau informacijos apie tai, kaip tai padaryti, rasite [konfigūruotina atpažinimo ženklų naudojimo "Microsoft" tapatybės platformoje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)informacija.
4. " **SAML" pagrįstos bendrosios autentifikacijos trikčių diagnostika**: rekomenduojame patikrinti [problemas, susijusias su "SAML" tipo autentifikacija konfigūruotose taikomosiose programose](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), kad rastumėte problemas, su kuriomis greičiausiai susidursite.
5. **Slaptažodžių pagrindu veikiančios bendrosios autentifikacijos trikčių diagnostika**: rekomenduojame patikrinti " [Azure AD" vienkartinio prisijungimo prie "Azure AD"](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)problemas, kad rastumėte problemas, su kuriomis greičiausiai susidursite.
6. Ryšio problemų naudojant VPN, rasite [kaip naudoti vieno prisijungimo (SSO) per VPN ir Wi-Fi ryšius](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
