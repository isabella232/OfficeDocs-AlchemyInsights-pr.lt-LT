---
title: OIDC pagrindo sklandžiosios bendrosios a prisijungimo (SSO) trikčių šalinimas
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105786"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC pagrindo sklandžiosios bendrosios a prisijungimo (SSO) trikčių šalinimas

- Norėdami sužinoti, kaip įtraukti OIDC pagrįstą programą į "Azure" nuomotoją, žr. ["Quickstart": "OIDC" pagrindu pagrįstos bendrosios autentis (SSO) taikomosios programos jūsų ""Azure Active Directory"" ("Azure AD") nuomotojo .](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Daugiau informacijos apie taikomąsias programas, kurios naudoja "OpenID Prisijungimas standarto bendrosios a sign-on, žr. Bendrosios a [sign-on OIDC pagrindo supratimas](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Informacijos, jei pasirinksite rašyti kodą tiesiogiai siųsdami ir tvarkant HTTP užklausas arba naudodami trečiosios šalies atvirojo kodo biblioteką, o ne naudodami vieną iš mūsų atvirojo kodo bibliotekų, [žr. "OAuth 2.0" ir "OpenID Prisijungimas" protokolai "Microsoft" tapatybės platforma](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokolai**

1. ["Microsoft" tapatybės platforma ir](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) netiesioginis grantų srautas – netiesioginės dotacijos apibrėžtis yra ta, kad atpažinimo ženklus (ID atpažinimo ženklus arba prieigos atpažinimo ženklus) grąžina tiesiogiai iš /authorize pabaigos taško, o ne iš /atpažinimo ženklo pabaigos taško. Tai dažnai naudojama kaip autorizavimo kodo srauto dalis, kas vadinama **"hibridiniu srautu" – nuskaito ID atpažinimo ženklą užklausoje /authorize kartu su įgaliojimo kodu.** Šiame straipsnyje aprašoma, kaip programuoti tiesiogiai pagal programos protokolą, kad būtų galima prašyti atpažinimo ženklų iš "Azure AD".
2. ["Microsoft" tapatybės platforma ir "OAuth 2.0"](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) autorizavimo kodo srautas – "OAuth 2.0" įgaliojimo kodo suteikimas gali būti naudojamas programose, įdiegtose įrenginyje norint gauti prieigą prie apsaugotų išteklių, pvz., žiniatinklio API. Naudodami ""Microsoft" tapatybės platforma OAuth 2.0", galite įtraukti prisijungimo ir API prieigą prie **mobiliųjų įrenginių ir darbalaukio programų.** Šiame straipsnyje aprašoma, kaip programuoti tiesiogiai pagal programos protokolą naudojant bet kurią kalbą.
3. ["Microsoft" tapatybės platforma "Prisijungimas" ir "OpenID"](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) protokolas – kai naudojate ""Microsoft" tapatybės platforma" "OpenID Prisijungimas", galite įtraukti prisijungimo ir API prieigą prie savo programų. Šiame straipsnyje aprašoma, kaip tai padaryti nepriklausomai nuo kalbos, ir aprašoma, kaip siųsti ir gauti **HTTP pranešimus nenaudojant jokių "Microsoft" atvirojo kodo bibliotekų.**
4. ["Microsoft" tapatybės platforma ir "OAuth 2.0"](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) kliento kredencialų srautą – galite naudoti "OAuth 2.0" kliento kredencialų grantą, nurodytą RFC 6749, kartais vadinamą dviejų dalių **"OAuth",** norėdami pasiekti žiniatinklio išteklius naudodami taikomosios programos tapatybę. Šis tipo grantas dažnai naudojamas sąveikai tarp serverio ir serverių, kurie turi veikti fone, be tiesioginio bendravimo su vartotojas. Šių tipų taikomosios programos dažnai vadinamos **demonais arba** tarnybos **paskyromis**. Šiame straipsnyje aprašoma, kaip programuoti tiesiogiai pagal jūsų taikomosios programos protokolą.
