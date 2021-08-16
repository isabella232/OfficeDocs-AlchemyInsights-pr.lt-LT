---
title: Sklandžių SSO integravimo su mano vietinėmis programėlėmis problemos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028300"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Sklandžių SSO integravimo su mano vietinėmis programėlėmis problemos

Norėdami šalinti sklandžių SSO integravimo su vietinėmis programomis problemas, atlikite šiuos veiksmus:

**Rekomenduojami veiksmai**

1. Norėdami **sukonfigūruoti vietinį** bendrosios autenčios taikomosios programos tarpinį serverį **,** žr. Bendrosios autentavimo naudojant taikomosios programos [tarpinį serverį slaptažodžių](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)saugyklos .
1. **Programos tarpinio serverio** trikčių šalinimas: rekomenduojame pradėti nuo trikčių šalinimo srauto [peržiūros,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)derinti taikomosios programos tarpinio serverio jungties problemas, kad nustatytumėte, ar tinkamai sukonfigūruotos taikomosios programos tarpinio serverio jungtys. Jei vis tiek kyla problemų jungiantis prie taikomosios programos, atlikite trikčių šalinimo veiksmus, nurodytus [Taikomosios programos tarpinio serverio taikomosios programos problemų derinimas.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Cors [problemas galite nustatyti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) naudodami šiuos naršyklės derinimo įrankius:
    1. Paleiskite naršyklę ir raskite žiniatinklio taikomąją programą.
    1. Paspauskite **F12,** kad iškeitų derinimo konsolė.
    1. Pabandykite atkurti operaciją ir peržiūrėkite konsolės pranešimą. CORS pažeidimas pateikia konsolės klaidą apie kilmę.
    1. Kai kurių CORS problemų išspręsti negalima, pvz., kai jūsų programa peradresuoja login.microsoftonline.com autentifikuoti, o prieigos atpažinimo ženklo galiojimas baigiasi. Tada CORS skambutis nepavyks. Šio scenarijaus sprendimo būdas yra pratęsti prieigos atpažinimo ženklo naudojimo laiką, kad jis truktų vartotojo seanso metu. Daugiau informacijos apie tai, kaip tai padaryti, žr. [Konfigūruojami atpažinimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)ženklų naudojimo "Microsoft" tapatybės platforma .

**Rekomenduojami dokumentai**

- [Kaip konfigūruoti bendrąją a prisijungimą prie taikomosios programos tarpinio serverio taikomosios programos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML bendroji a prisijungimo prie vietinės taikomosios programos su taikomosios programos tarpinis serveris](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- ["Application Proxy CORS"Azure Active Directory" problemų supratimas ir sprendimas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- ["Kerberos" apriboto perdavimo konfigūracijų trikčių šalinimas naudojant programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)