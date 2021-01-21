---
title: "\"Tokens\" problemos"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917040"
---
# <a name="issues-with-tokens"></a>"Tokens" problemos

Norėdami tvarkyti su atpažinimo ženklų problemas, galite atlikti šiuos veiksmus:

1. Galite apibrėžti "Microsoft" tapatybės platformos išduoto prieigos, ID arba SAML atpažinimo ženklo galiojimo laiką. Galite nustatyti atpažinimo ženklų naudojimo visas savo organizacijos taikomąsias programas, kelių nuomotojų (kelių organizacijų) taikomąją programą arba konkrečią organizacijos pagrindinę tarnybą. Daugiau informacijos ieškokite ["Microsoft" tapatybės platformoje konfigūruojamų atpažinimo ženklų naudojimo laiko (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. "Access" žetonai leidžia klientams saugiai skambinti apsaugotą žiniatinklio API ir juos naudoja žiniatinklio API, kad galėtų atlikti autentifikavimą ir autorizavimą. Kaip ir OAuth specifikacija, "Access" žetonai yra nepermatomos eilutės, nenaudojant rinkinio formato – kai kurie tapatybės teikėjai (IDPs) naudoja GUID, kiti naudoja užšifruotą BLOB. "Microsoft" tapatybės platformoje naudojami įvairūs "Access" atpažinimo ženklų formatai, atsižvelgiant į tai, kaip API konfigūracija priima atpažinimo ženklą. Norėdami sužinoti, kaip jūsų API gali patvirtinti ir naudoti "Access" atpažinimo ženklo teiginius, peržiūrėkite ["Microsoft" tapatybės platformos prieigos žetonus](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. "Microsoft" autentifikavimo biblioteka (MSAL) palaiko kelis autentifikavimo srautus, skirtus naudoti skirtinguose taikomosios programos scenarijuose. Daugiau informacijos ieškokite [autentifikavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. "OAuth 2,0" autorizavimo kodo dotaciją galima naudoti įrenginyje įdiegtose programėlėse, norint gauti prieigą prie apsaugotų išteklių, pvz., žiniatinklio API. Naudodami "Microsoft" tapatybės platformos "OAuth 2,0" diegimą, galite įtraukti prisijungimo ir API prieigą prie mobiliųjų įrenginių ir kompiuterio taikomųjų programų. Peržiūrėkite ["Microsoft" tapatybės platformą ir "OAuth" 2,0 autorizavimo kodo srautą](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) , kaip tiesiogiai programos protokolą programoje, naudojant bet kurią kalbą.
5. OpenID Connect (OIDC) yra autentifikavimo protokolas, sukurtas "OAuth 2,0", kurį galite naudoti norėdami saugiai prisijungti vartotojui į taikomąją programą. Kai naudojate "Microsoft" tapatybės platformos galinio punkto "OpenID Connect" įdiegtį, galite įtraukti prisijungimo ir API prieigą prie savo taikomųjų programų. Naudojant ["Microsoft" tapatybės platformą ir "OpenID Connect" protokolą](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) rodoma, kaip tai padaryti nepriklausomai nuo kalbos ir aprašoma, kaip siųsti ir gauti http pranešimą nenaudojant jokių "Microsoft" atvirosios šaltinio bibliotekų.
    - UserInfo galinis punktas yra OIDC standarto dalis, skirta pateikti teiginius apie autentifikuotą vartotoją. Daugiau informacijos ieškokite ["Microsoft" tapatybės platformos UserInfo galinio punkto](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Žiniatinklio taikomosios programos [Skambinimas žiniatinklio API naudojant "AZURE AD" ir "OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) " pavyzdys rodo, kaip kurti MVC žiniatinklio taikomąją programą, kuri naudoja "Azure AD" prisijungimui naudodami "OpenID Connect" protokolą, o tada paskambinti žiniatinklio API pagal vartotojo tapatybę, naudodami atpažinimo ženklus, gautus naudojant "oauth 2,0". Šis pavyzdys naudoja OpenID Connect ASP .net OWIN tarpinės ir adal .net.
6. [Konfigūruokite taikomąją programą, kad būtų galima atskleisti žiniatinklio API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – šiame "QuickStart" užregistruojate žiniatinklio API naudodami "Microsoft" tapatybės platformą ir įtraukite ją į kliento taikomąsias programas įtraukdami pavyzdžio aprėptį. Registruodami žiniatinklio API ir naudodami aprėptis, galite suteikti teisėmis pagrįstą prieigą prie jos išteklių įgaliotiems vartotojams ir kliento programoms, kurios pasiekia jūsų API.
7. "Azure Active Directory" B2C ("Azure AD B2C") išteklių savininko slaptažodžio kredencialus (ROPC) srautas yra OAuth Standard autentifikavimo srautas. Šiame sraute taikomoji programa, taip pat žinoma kaip besiremianti šalis, leidžia naudoti "Tokens" leistinus kredencialus. Kredencialai apima vartotojo ID ir slaptažodį. Pateikti žetonai yra ID atpažinimo ženklas, prieigos žetonas ir atnaujinimo atpažinimo ženklas. Daugiau informacijos ieškokite [išteklių savininko slaptažodžio kredencialų srauto nustatymas "Azure Active Directory" B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

