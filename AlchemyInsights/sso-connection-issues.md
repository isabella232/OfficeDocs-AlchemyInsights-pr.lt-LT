---
title: SSO ryšio problemos
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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084354"
---
# <a name="sso-connection-issues"></a>SSO ryšio problemos

1. Vykdykite ["Quickstart": konfigūruokite taikomosios programos vadovo](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ypatybes, kad konfigūruokite taikomąją programą.
2. Atsižvelgiant į jūsų pasirinktą taikomąją programą ir [bendrąją a prisijungimo](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) parinktį, vadovaukitės toliau pateikiamomis atitinkamomis gairėmis:
    - Norėdami **sukonfigūruoti vietinę** taikomąją programą SAML pagrindu sukurtoms bendrosios **ausinių** ausims , žr. SAML bendrosios a sign-on vietinės taikomosios programos su [taikomosios programos tarpinis serveris](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Norėdami sukonfigūruoti **debesies taikomąją** **programą slaptažodžiu pagrįstai bendrosios adresą**,  [žr. Bendrosios a prisijungimo prie slaptažodžio konfigūravimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Norėdami **sukonfigūruoti vietinį** bendrosios autenčios taikomosios programos tarpinį serverį **,** žr. Bendrosios autentavimo naudojant taikomosios programos [tarpinį serverį slaptažodžių](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)saugyklos .
3. **Programos tarpinio serverio** trikčių šalinimas: rekomenduojame pradėti nuo trikčių šalinimo srauto [peržiūros,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)derinti taikomosios programos tarpinio serverio jungties problemas, kad nustatytumėte, ar tinkamai sukonfigūruotos taikomosios programos tarpinio serverio jungtys. Jei vis tiek kyla problemų jungiantis prie taikomosios programos, vykdykite trikčių šalinimo srautą derinimo taikomosios [programos tarpinio serverio taikomosios programos problemose.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Cors [problemas galite nustatyti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) naudodami naršyklės derinimo įrankius:
    - Paleiskite naršyklę ir raskite žiniatinklio taikomąją programą.
    - Paspauskite **F12,** kad iškeitų derinimo konsolė.
    - Pabandykite atkurti operaciją ir peržiūrėkite konsolės pranešimą. CORS pažeidimas pateikia konsolės klaidą apie kilmę.
    - Kai kurių CORS problemų išspręsti negalima, pvz., kai jūsų programa peradresuoja login.microsoft.com autentifikuoti, o prieigos atpažinimo ženklas baigia galioti. Tada CORS skambutis nepavyks. Šio scenarijaus sprendimo būdas yra pratęsti prieigos atpažinimo ženklo naudojimo laiką, kad jis truktų vartotojo seanso metu. Daugiau informacijos apie tai, kaip tai padaryti, žr. [Konfigūruojami atpažinimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)ženklų naudojimo "Microsoft" tapatybės platforma .
4. Saml pagrįstos bendrosios a **sign-on** trikčių šalinimas: rekomenduojame patikrinti Prisijungimo prie [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)pagrindu sukonfigūruotas bendrosios afiksavimo programos problemas, kad rastumėte problemų, su kuriomis greičiausiai susiduriate, sprendimus.
5. **Bendrosios a prisijungimo** prie slaptažodžio trikčių šalinimas: rekomenduojame patikrinti Slaptažodžio pagrindu pagrįstos bendrosios a prisijungimo trikčių šalinimas naudojant ["Azure AD",](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)kad rastumėte problemų, su kuriomis greičiausiai susiduriate, sprendimus.
6. Ryšio problemų naudojant VPN žr. Kaip naudoti bendrąją jungtį [(SSO) naudojant VPN ir Wi-Fi ryšius](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
