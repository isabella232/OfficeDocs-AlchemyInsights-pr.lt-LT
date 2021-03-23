---
title: "\"OAuth 2,0\" ir \"OpenID Connect\" protokolų trikčių diagnostika"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036403"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>"OAuth 2,0" ir "OpenID Connect" protokolų trikčių diagnostika

Norėdami išspręsti "OAuth 2,0" ir "OpenID Connect" problemas, atlikite šiuos rekomenduojamus veiksmus:

Peržiūrėkite šiuos straipsnius, susijusius su konfigūravimu ir trikčių diagnostika "OAuth 2,0" ir "OpenID Connect" protokolai:

- ["Microsoft" tapatybės platforma ir "OAuth" 2,0 autorizavimo kodo srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – šiame straipsnyje aprašyta, kaip programa tiesiogiai su **kodo suteikimo (pkce) srautu** taikomąja programa, naudojant bet kurią kalbą.
- ["Microsoft" tapatybės platforma ir "OAuth 2,0" kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – šiame straipsnyje aprašyta, kaip programa tiesiogiai **kliento kredencialų srautui** taikomojoje programoje.
- ["Microsoft" tapatybės platforma ir "OAuth 2,0" išteklių savininko slaptažodžio kredencialai](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – šiame straipsnyje aprašyta, kaip programa tiesiogiai su " **ropc" srautu** taikomojoje programoje.
    - "Microsoft Identity" platforma palaiko tik "ROPC", skirtą "Azure AD" nuomininkams, o ne asmeniniams abonementams. Tai reiškia, kad turite naudoti konkretaus nuomotojo galinį punktą **( https://login.microsoftonline.com/{TenantId_or_Name})** arba **organizacijos** galinį punktą.
    - Asmeninės paskyros, kviečiamos į "Azure AD" nuomotoją, negali naudoti "ROPC".
    - Paskyros, kuriose nėra slaptažodžių, negali prisijungti per ROPC. Pagal šį scenarijų rekomenduojame naudoti skirtingą programos srautą.
    - Jei vartotojai turi naudoti [kelių dalių autentifikavimą (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) , kad prisijungtų prie taikomosios programos, jie bus užblokuoti.
    - ROPC nepalaikoma [hibridinės tapatybės susiejimo](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) scenarijuose (pvz., "Azure AD" ir ADFS, naudojami vietinėms paskyroms autentifikuoti). Jei vartotojai yra visame puslapyje nukreipiami į vietinį tapatybės teikėją, "Azure AD" negali patikrinti vartotojo vardo ir slaptažodžio prieš tą tapatybės teikėją. [Pass-per autentifikavimo](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) palaikomas su ropc, tačiau.
    - Hibridinis tapatybės susiejimo scenarijų išimtis būtų tokia: "Home Realm" aptikimo strategija naudojant " **Allowcloudpasswordvalidation** " reikšmę **True** įgalins "ropc" srautą, jei norite dirbti su išoriniu vartotoju, kai vietinis slaptažodis sinchronizuojamas su debesimi. Daugiau informacijos ieškokite skyriuje [tiesioginių "ROPC" išorinių vartotojų autentifikavimas naudojant senstelėjusias taikomąsias programas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- ["Microsoft" tapatybės platforma ir "OAuth 2,0" srauto vardu](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – šiame straipsnyje aprašyta, kaip programa tiesiogiai **(OBO) srautui** taikomojoje programoje.
- ["Microsoft" tapatybės platformos ir "OpenID Connect" protokolas](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – šiame straipsnyje parodyta, kaip įdiegti "OpenID Connect" protokolą nepriklausomai nuo kalbos ir aprašoma, kaip siųsti ir gauti http pranešimą nenaudojant jokių "Microsoft" atvirosios šaltinio bibliotekų.

**"Access" žetonai**

["Microsoft" tapatybės platformos prieigos žetonai](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Sužinokite, kaip jūsų API gali patvirtinti ir naudoti "Access" atpažinimo ženklo teiginius. Visi šiame straipsnyje nurodyti dokumentai, išskyrus tuos atvejus, kai pažymėta, taikomi tik žetonams, kurie buvo išduoti jūsų įregistruotam API. Jis netaikomas žetonams, išduodamais "Microsoft" valdomoms API, taip pat šie žetonai negali būti naudojami norint patikrinti, kaip "Microsoft" tapatybės platforma pateiks Jūsų kuriamos API atpažinimo ženklus.

**Taikomosios programos konfigūracija**

[Peradresavimo URI (atsakymo URL) apribojimai ir apribojimai](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Sužinokite, kaip SUKONFIGŪRUOTI peradresavimo URI (atsakymo URL). Peradresavimo URI arba atsakymo URL yra vieta, kurioje autorizuotas serveris siunčia vartotoją, kai programa sėkmingai autorizuotas ir jai suteiktas autorizavimo kodas arba prieigos žetonas. Autorizavimo serveris siunčia kodą arba žetoną į peradresavimo URI; Todėl svarbu užregistruoti tinkamą vietą kaip programos registracijos proceso dalį.

**Taikomosios programos parengimas**

[Vadovėlis: kurti ir planuoti parengimo "SCIM" galinį punktą](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – šiame straipsnyje aprašoma, kaip sukurti "SCIM" galinį punktą ir integruoti su "AAD" parengimo tarnyba.


