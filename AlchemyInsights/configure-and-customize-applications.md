---
title: Taikomųjų programų konfigūravimas ir tinkinimas
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063659"
---
# <a name="configure-and-customize-applications"></a>Taikomųjų programų konfigūravimas ir tinkinimas

**Taikomųjų programų konfigūravimas**

1. " [QuickStart": konfigūruokite taikomosios programos ypatybes "Azure Active Directory" ("AZURE AD") nuomotojuje](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) rodoma, kaip konfigūruoti kai kurias programos ypatybes.
2. Kad būtų lengviau integruoti taikomąsias programas su "Azure Active Directory", sukūrėme [mokomųjų programų rinkinį](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) , kurį galite atlikti naudodami konfigūraciją.
3. [Kaip sukonfigūruoti taikomosios programos tarpinio serverio taikomąją](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programą padeda suprasti, kaip sukonfigūruoti taikomosios programos tarpinio serverio taikomąją programą "Azure AD", kad jūsų vietinėms programoms būtų rodoma debesyje.
4. [Atsisiųskite "PingAccess" ir Konfigūruokite savo taikomąją programą](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): vadovaukitės instrukcijomis, pateiktomis *Konfigūruokite Pingaccess "Azure AD", kad apsaugotų taikomąsias programas* , publikuotas naudojant "Microsoft Azure AD Application proxy" "Ping Identity" žiniatinklio svetainėje, ir atsisiųsti naujausią "pingaccess

**Netinkamai sukonfigūruota taikomosios programos (AADSTS650056) klaidos**

1. Įsitikinkite, kad pasiekiate taikomąją programą iš programos savininko pateikto prisijungimo adreso. Kitu atveju Prisijunkite prie taikomosios programos naudodami įprastą procesą. Daugeliu atvejų tai bus automatiškai išspręsta natūraliai. Jei ne, šis skelbimas gali padėti išspręsti ir išspręsti problemą.
2. **Jei jūsų organizacija turi taikomąją programą** (reiškianti taikomosios programos registraciją jūsų organizacijoje):
    - Minimaliai rekomenduojame `User.Read` `openid` įtraukti arba įgaliotasis teises iš **"Microsoft Graph** ".
    - Įsitikinkite, kad sutinkate su taikomąja programa ir visomis jos teisėmis. Galite tai patikrinti peržiūrėdami taikomosios programos " **API" teisių** stulpelį **Būsena** .
    - Kai kuriuose scenarijuose taikomoji programa gali būti trečiosios šalies, tačiau ji gali būti registruota jūsų organizacijoje. Patvirtinkite, kad Ši taikomoji programa pateikta jūsų taikomųjų programų registracijose (ne įmonės taikomosios programos).
    - Jei ir toliau matysite šį klaidos pranešimą. Tada gali tekti sukurti **4 veiksme** aprašytą sutikimo URL.
3. **Jei jūsų organizacija nėra programos savininkas ir naudoja ją kaip trečiosios šalies taikomąją programą**:
    - Jei esate pasaulinis/įmonės administratorius, turėtumėte matyti sutikimo ekraną. Įsitikinkite, kad žymės langelį **"sutikimas organizacijos vardu"**.
    - Jei nematote lango sutikimas, panaikinkite įmonės taikomąją programą ir bandykite dar kartą.
    - Jei ir toliau matysite šį klaidos pranešimą. Tada gali tekti sukurti **4 veiksme** aprašytą sutikimo URL.
4. **Rankiniu būdu sukurkite naudojamo sutikimo URL**: jei taikomoji programa skirta pasiekti konkretų šaltinį, jums gali nepavykti naudoti sutikimo mygtukų iš "Azure" portalo, todėl turėsite rankiniu būdu sugeneruoti savo sutikimo URL ir jį naudoti.
    - Jums reikės gauti `{App-Id}` ir `{App-Uri-Id}` iš programos savininko. `{Tenant-Id}` bus jūsų nuomotojo identifikatorius. Tai bus `yourdomain.onmicrosoft.com` arba jūsų katalogo ID.
    - Jei taikomoji programa jungiasi prie išteklių, tada `{App-Id}` `{App-Uri-Id}` bus tas pats.
5. Daugiau informacijos ieškokite [problemų prisijungiant prie SAML pagrįstų vienkartinio prisiregistravimo konfigūruojamų taikomųjų programų](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Taikomųjų programų tinkinimas**

- [Įtraukite prekės ženklų į savo organizacijos "Azure Active Directory" prisijungimo puslapį](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – naudokite organizacijos logotipą ir pasirinktinę spalvų schemas, kad galėtumėte nuosekliai peržvelgti savo "Azure Active Directory" ("Azure AD") prisijungimo puslapius.
- [Pasirinktinio domeno vardo įtraukimas naudojant "Azure Active Directory" portalą](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – kiekvienas naujas "Azure AD" nuomotojas pateikiamas su pirminiu domeno vardu. Negalite keisti arba panaikinti pradinio domeno vardo, tačiau galite įtraukti savo organizacijos pavadinimus. Įtraukus pasirinktinio domenų vardus, lengviau kurti vartotojų vardus, kurie yra susipažinę su vartotojais.
