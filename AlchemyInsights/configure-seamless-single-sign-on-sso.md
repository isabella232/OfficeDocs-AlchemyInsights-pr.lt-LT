---
title: Vientiso vienkartinio prisijungimo (SSO) konfigūravimas
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841535"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Vientiso vienkartinio prisijungimo (SSO) konfigūravimas

**Taikomųjų programų konfigūravimas**

1. Turite gauti reikšmes iš taikomosios programos tiekėjo. Galite neautomatiniu būdu įvesti reikšmes arba nusiųsti metaduomenų failą, kad išskleistumėte laukų reikšmę.
2. Daugelis programų jau buvo iš anksto sukonfigūruotos veikti su "Azure AD". Šios taikomosios programos pateiktos programų galerijoje, kurią galite naršyti įtraukdami taikomąją programą į "Azure AD" nuomotoją. " [QuickStart" seka](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) jūsų procesas.
3. Norėdami sukurti ne galerijos taikomąją programą, galite spustelėti "+" **kurti savo taikomosios** programos mygtuką ir suteikti programai pavadinimą.
    - Pagal numatytuosius, ji pasirinks **įtraukti bet kurią kitą taikomąją programą** , kurios nerandate galerijoje, kuri yra tinkama parinktis ne galerijos programoms.
    - Kai paspausite **kurti** po taikomosios programos pavadinimo, ji sukurs naują ne galerijos įmonės taikomąją programą.
    - Tada galite pereiti prie **bendrosios autentifikacijos** dalyje **valdyti** šią taikomąją programą ir galėsite matyti skirtingus jos įgyvendinimo būdus savo aplinkoje.

**"Besiūlių SSO" konfigūravimas konkrečiai taikomajai programai**

Galerijoje esančios programos pateikiamos išsamios ir nuoseklios instrukcijos. Norėdami pasiekti veiksmus, galite naršyti visų taikomųjų programų konfigūravimo mokomųjų programų sąrašą " [SaaS" taikomųjų programų konfigūravimo vadovuose](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**SAML pagrindo SSO konfigūravimas**

1. [Greitoji paleistis: SAML pagrįstos bendrosios autentifikacijos (SSO), skirtos "Azure Active Directory" ("AZURE AD") nuomotojuje, nustatymas](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Jei norite sužinoti daugiau apie SAML pagrįstą parinktį, skirtą vienkartiniam autentifikacija, skaitykite " [SAML" pagrįstos bendrosios autentifikacijos supratimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Norėdami sužinoti apie "SAML 2,0" autentifikavimo užklausas ir atsakymus, kad "Azure Active Directory" ("Azure AD") palaiko vieną Sign-On (SSO), peržiūrėkite [vieną Sign-On SAML protokolą](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Norėdami sužinoti, kaip kurti ir konfigūruoti savo taikomosios programos bendrosios autentifikacijos (SSO) "Azure Active Directory" ("Azure AD"), naudojant "Microsoft Graph" API, peržiūrėkite [savo taikomajai programai skirtos bendrosios autentifikacijos konfigūravimą naudojant "Microsoft Graph" API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Norėdami sužinoti, kaip "Azure AD" naudoja SAML protokolą, Sužinokite, [kaip "Microsoft" tapatybės platforma naudoja SAML protokolą](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Žetonų ir pretenzijų konfigūravimas**

1. [Kaip: tinkinti reikalavimus, pateiktus "SAML" atpažinimo ženklo įmonėms taikomosiose programose](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Norėdami sužinoti, kaip konfigūruoti reikalavimus naudojant "PowerShell", Sužinokite, [kaip: tinkinti teiginius, kurie yra išmetami su konkrečios programos nuomotojuje (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Norėdami sužinoti, kaip konfigūruoti neprivalomus teiginius, Sužinokite, [kaip: pateikti pasirinktines savo taikomosios programos pretenzijas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Norėdami sužinoti, kaip naudoti katalogo schemos plėtinio atributus, kad būtų galima siųsti vartotojų duomenis į taikomąsias programas atpažinimo ženklų ieškiniams, skaitykite " [Directory" schemos plėtinio atributų naudojimas ieškiniams](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Norėdami sužinoti, kaip sukonfigūruoti atpažinimo ženklų naudojimo laiką, peržiūrėkite ["Microsoft" tapatybės platformos (Preview) konfigūruotinas atpažinimo ženklų naudojimo laikas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfigūruokite atpažinimo ženklo naudojimo strategijas (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – šiame straipsnyje mes peržiūrime bendrą strategijos scenarijų, kuris gali padėti nustatyti naujas taisykles simboliniams gyvavimo laikui. Pavyzdyje sužinosite, kaip sukurti strategiją, pagal kurią vartotojai turi dažniau autentifikuoti jūsų žiniatinklio taikomąją programą.

**SSO konfigūracijos trikčių šalinimas**

- Dažnai užduodamų klausimų apie "Azure Active Directory" vientisas Sign-On (besiūlių SSO) ieškokite " [Azure Active Directory" vientisas autentifikacijos: dažnai užduodami klausimai](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Trikčių diagnostikos informacijos apie įprastas problemas, susijusias su "Azure Active Directory" ("Azure AD"), vientiso Sign-On (besiūlių SSO) ieškokite " [Azure Active Directory" sklandžios bendrosios autentifikacijos trikčių diagnostika](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
