---
title: Sklandžiosios bendrosios a sign-on (SSO) konfigūravimas
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
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966045"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Sklandžiosios bendrosios a sign-on (SSO) konfigūravimas

**Programų konfigūravimas**

1. Reikšmes turėtumėte gauti iš taikomosios programos tiekėjo. Galite rankiniu būdu įvesti reikšmes arba nusiųsti metaduomenų failą, kad išskleistų laukų reikšmę.
2. Daugelis programų jau iš anksto sukonfigūruotos veikti su "Azure AD". Šios programos išvardytos programų galerijoje, kurią galite naršyti įtraukdami programą į "Azure AD" nuomotoją. [Spartusis sekų](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) sekų vaikščios jus per procesą.
3. Norėdami sukurti ne galerijos taikomąją programą, galite spustelėti + Kurti **savo** taikomąją programą ir suteikti savo taikomosios programos pavadinimą.
    - Pagal numatytuosius nustatymus bus **parinktis** Integruoti bet kurią kitą taikomąją programą, kurios nerandate galerijoje, kuri yra tinkama parinktis ne galerijos programoms.
    - Kai paspausite **Kurti** po to, kai įdėsite taikomosios programos pavadinimą, bus sukurta nauja ne galerijos "Enterprise" taikomoji programa.
    - Tada galite pereiti prie **bendrosios ausinės** dalyje Tos taikomosios programos valdymas ir galėsite matyti skirtingus būdus, kaip ją įgyvendinti savo aplinkoje. 

**Sklandžias SSO konfigūravimas konkrečiai programai**

Galerijoje pateikiamų programėlių išsamias, išsamias, išsamias instrukcijas. Norėdami pasiekti veiksmus, galite naršyti visų programų konfigūravimo mokymo priemonių sąrašą [saaS programos konfigūravimo mokymo priemonėse.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML pagrindo SSO konfigūravimas**

1. ["Quickstart": nustatykite "SAML" pagrįstą bendrąją autentisfikuoti (SSO) savo ""Azure Active Directory" ("Azure AD") nuomotojui.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Norėdami sužinoti daugiau apie saml pagrįstą bendrosios afikso parinkties informaciją, žr. [Saml pagrindu sukurto bendrosios a prisijungimo informacijos supratimas.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Norėdami sužinoti apie SAML 2.0 autentifikavimo užklausas ir atsakymus, kuriuos ""Azure Active Directory"" ("Azure AD") palaiko "Single Sign-On" (SSO), žr. ["Single Sign-On SAML" protokolas](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Norėdami sužinoti, kaip kurti ir konfigūruoti ""Azure Active Directory"" ("Azure AD") programos SAML pagrįstą bendrąją afiksą (SSO) naudojant "Microsoft "Graph" API", žr. SAML pagrindu pagrįstos bendrosios a prisijungimo prie programos konfigūravimas naudojant ["Microsoft "Graph" API".](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Norėdami sužinoti, kaip "Azure AD" naudoja SAML protokolą, [žr. Kaip "Microsoft" tapatybės platforma naudoja SAML protokolą.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Atpažinimo ženklų ir pretenzijų konfigūravimas**

1. [Kaip: tinkinti pretenzijas, išduotas "SAML" atpažinimo ženklu, skirtame įmonės programoms.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Norėdami sužinoti, kaip konfigūruoti pretenzijas naudojant "PowerShell", žr. Kaip: Tinkinkite pretenzijas, [išmestas žetonuose, tam tikroje nuomotojo taikomojoje programoje (peržiūra).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Norėdami sužinoti, kaip konfigūruoti pasirinktines pretenzijas, [žr. Kaip: Pateikti pasirinktinius teiginius savo programai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Norėdami sužinoti, kaip naudoti katalogų schemos plėtinių atributus siunčiant vartotojo duomenis į taikomąsias programas atpažinimo ženklų teiginiuose, [žr. Katalogų schemos plėtinių atributų naudojimas pretenzijose](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Norėdami sužinoti, kaip konfigūruoti atpažinimo ženklų naudojimo laikotarpius, žr. Konfigūruojami atpažinimo [ženklų naudojimo "Microsoft" tapatybės platforma (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfigūruokite atpažinimo ženklo](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) naudojimo trukmės strategijas (peržiūra) – šiame straipsnyje peržiūrėsime bendrą strategijos scenarijų, kuris gali padėti nustatyti naujas atpažinimo ženklo naudojimo trukmės taisykles. Pavyzdyje sužinosite, kaip sukurti strategiją, pagal kurią vartotojai turi dažniau autentifikuoti žiniatinklio programoje.

**SSO konfigūravimo trikčių šalinimas**

- Dažnai užduodamų klausimų apie ""Azure Active Directory" Single Sign-On" (sklandų SSO) žr. "Azure Active Directory" Vientisa bendroji [a prisijungimo informacija: dažnai užduodami klausimai](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Informacijos apie įprastas ""Azure Active Directory" ("Azure AD") sklandžias viengules "Sign-On" (sklandžias SSO) triktis žr. ""Azure Active Directory" Vientisos bendrosios [a prisijungimo trikčių šalinimas.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
