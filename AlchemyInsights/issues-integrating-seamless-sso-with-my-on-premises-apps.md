---
title: Problemos, susijusios su besiūlių SSO integravimu su mano vietinėje programėlėmis
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868717"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemos, susijusios su besiūlių SSO integravimu su mano vietinėje programėlėmis

Norėdami šalinti triktis, susijusias su sklandžiais SSO integravimu su vietinėse taikomosiose programose, atlikite šiuos veiksmus:

**Rekomenduojami veiksmai**

1. Norėdami sukonfigūruoti **vietinę taikomąją** programą, skirtą **vienkartiniam autentifikacija naudojant taikomosios programos tarpinį serverį**, peržiūrėkite [bendrosios autentifikacijos slaptažodį naudojant taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Taikomųjų programų tarpinio serverio problemų trikčių diagnostika**: rekomenduojame pradėti peržiūrėti trikčių šalinimo srautą, [derinti taikomosios programos tarpinio serverio jungties problemas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), kad nustatytumėte, ar taikomosios programos tarpinio serverio jungtys tinkamai sukonfigūruotos. Jei vis dar kyla problemų jungiantis prie taikomosios programos, vadovaukitės trikčių šalinimo veiksmais [derinimo taikomosios programos tarpinio serverio taikomosios programos problemoms spręsti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). " [CORS" problemas galite identifikuoti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) naudodami šiuos naršyklės derinimo įrankius:
    1. Paleisk naršyklę ir naršykite į žiniatinklio programą.
    1. Paspauskite **F12** , kad iškviestumėte derinimo konsolę.
    1. Pabandykite atkurti operaciją ir peržiūrėkite konsolės pranešimą. CORS pažeidimas sukuria konsolės klaidą apie kilmę.
    1. Kai kurios "CORS" problemos neišsprendžiamos, pvz., kai jūsų programa nukreipia į "login.microsoftonline.com" ir "Access" atpažinimo ženklo galiojimo laikas baigsis. Tada nepavyksta. Šio scenarijaus sprendimo būdas – pratęsti "Access" atpažinimo ženklo galiojimo laiką, kad jis nesibaigtų vartotojo seanso metu. Daugiau informacijos apie tai, kaip tai padaryti, rasite [konfigūruotina atpažinimo ženklų naudojimo "Microsoft" tapatybės platformoje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)informacija.

**Rekomenduojami dokumentai**

- [Kaip sukonfigūruoti bendrąją autentifikacija taikomosios programos tarpinio serverio taikomajai programai](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML vienkartinė autentifikacija vietinėms programoms naudojant taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- ["Azure Active Directory" taikomųjų programų tarpinio serverio problemų supratimas ir sprendimas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- ["Kerberos" ribojami taikomųjų programų tarpinio serverio perdavimo konfigūracijų trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)