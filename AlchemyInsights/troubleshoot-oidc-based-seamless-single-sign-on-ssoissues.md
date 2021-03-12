---
title: OIDC pagrįstos vientisos vienkartinio prisijungimo (SSO) trikčių šalinimas
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
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747124"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC pagrįstos vientisos vienkartinio prisijungimo (SSO) trikčių šalinimas

- Norėdami sužinoti, kaip įtraukti OIDC pagrįstą taikomąją programą į savo "Azure" nuomotoją, skaitykite " [QuickStart": "oidc" pagrįstos vienkartinio prisijungimo (SSO) taikomosios programos, skirtos "Azure Active Directory" ("AZURE AD") nuomotojuje, nustatymas](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Daugiau informacijos apie taikomąsias programas, kurios naudoja "OpenID Connect Standard", Norėdami įgyvendinti bendrąją autentifikacijos funkciją, rasite ["OIDC" pagrįstos bendrosios autentifikacijos supratimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Jei norite gauti informacijos, jei norite rašyti kodą tiesiogiai siųsdami ir tvarkydami HTTP užklausas arba naudodami trečiosios šalies atvirosios šaltinio biblioteką, o ne naudodami vieną iš mūsų atidarytų šaltinių bibliotekų, peržiūrėkite ["OAuth 2,0" ir "OpenID Connect" protokolus "Microsoft" tapatybės platformoje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokolai**

1. ["Microsoft" tapatybės platforma ir numanomas dotacijos srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – netiesioginės dotacijos ypatybė yra ta, kad žetonai (ID žetonai arba prieigos žetonai) grąžinami tiesiogiai iš/įgalioti galinio punkto vietoj/atpažinimo ženklo galinio punkto. Tai dažnai naudojama kaip leidimo kodo srauto dalis, kas vadinama **hibridiniu srautu – nuskaitant ID atpažinimo ženklą, esantį užklausoje/įgalioti, kartu su autorizavimo kodu**. Šiame straipsnyje aprašyta, kaip programa tiesiogiai pagal jūsų taikomosios programos protokolą prašyti žetonų iš "Azure AD".
2. ["Microsoft" tapatybės platforma ir "oauth 2,0" autorizavimo kodo srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – "oauth 2,0" autorizavimo kodo dotacija galima naudoti įrenginyje įdiegtose programėlėse, norint gauti prieigą prie apsaugotų išteklių, pvz., žiniatinklio API. Naudodami "Microsoft" tapatybės platformos "OAuth 2,0" diegimą, galite **Įtraukti prisijungimo ir API prieigą prie mobiliųjų įrenginių ir kompiuterio taikomųjų programų**. Šiame straipsnyje aprašyta, kaip programa tiesiogiai atitinka jūsų taikomosios programos protokolą, naudojant bet kurią kalbą.
3. ["Microsoft" tapatybės platforma ir "OpenID Connect" protokolas](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – kai naudojate "Microsoft" tapatybės platformos "OpenID Connect" diegimą, galite įtraukti prisijungimo ir API prieigą prie savo taikomųjų programų. Šiame straipsnyje parodyta, kaip tai padaryti nepriklausomai nuo kalbos ir aprašoma, kaip **Siųsti ir gauti http laišką nenaudojant jokių "Microsoft" atvirosios šaltinio bibliotekų**.
4. ["Microsoft" tapatybės platforma ir "oauth 2,0" kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – galite naudoti "oauth 2,0" kliento kredencialų dotaciją, nurodytą rfc 6749, kartais vadinamą **Two-legged OAuth**, kad pasiektumėte žiniatinklio išteklius naudodami taikomosios programos tapatumą. Šio tipo dotacija paprastai naudojama atliekant serverio ir serverio sąveikas, kurios turi veikti fone, be tiesioginių sąveikų su vartotoju. Šie taikomųjų programų tipai dažnai vadinami " **daemons** " arba " **Service" paskyromis**. Šiame straipsnyje aprašyta, kaip programa tiesiogiai atitinka jūsų taikomosios programos protokolą.
