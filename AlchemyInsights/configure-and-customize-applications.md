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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044996"
---
# <a name="configure-and-customize-applications"></a>Taikomųjų programų konfigūravimas ir tinkinimas

**Programų konfigūravimas**

1. ["Quickstart": ""Azure Active Directory" ("Azure AD")](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) nuomotojo taikomosios programos ypatybės rodo, kaip konfigūruoti kai kurias programos ypatybes.
2. Norėdami padėti integruoti programas su "Azure Active Directory", sukūrėme mokomųjų programų [rinkinį, kuris](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) padės jums konfigūruoti.
3. [Kaip konfigūruoti taikomosios programos tarpinio serverio](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) taikomąją programą, galima suprasti, kaip konfigūruoti taikomosios programos tarpinio serverio taikomąją programą "Azure AD", kad jūsų vietinės taikomosios programos būtų pateiktos debesyje.
4. [Atsisiųskite "PingAccess"](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)ir konfigūruokite taikomąją programą: vykdykite nurodymus, pateiktus *"Azure AD" "PingAccess" konfigūravimas,* kad apsaugotumėte programas, publikuotas naudojant ""Microsoft Azure AD" Application Proxy" "Ping Identity" žiniatinklio svetainėje ir atsisiųskite naujausią "PingAccess" versiją.

**Netinkamai sukonfigūruota taikomoji programa (AADSTS650056) klaidos**

1. Įsitikinkite, kad naudojate taikomąją programą naudodami prisijungimo adresą, kurį pateikė taikomosios programos savininkas. Kitu atveju prisijunkite prie taikomosios programos per įprastą procesą. Daugeliu atvejų tai automatiškai išspręs natūraliai. Jei taip nėra, šis įrašas gali padėti pašalinti triktis ir išspręsti problemą.
2. **Jei jūsų organizacijai priklauso programa (tai** reiškia, kad taikomosios programos registracija yra jūsų organizacijoje):
    - Bent jau rekomenduojame įtraukti "Microsoft "Graph" arba `User.Read` `openid` **įgaliotas** teises.
    - Įsitikinkite, kad taikomoji programa ir visos jos teisės yra duotos. Tai galite patikrinti peržiūrėę programos **registracijos** stulpelį Būsena API **teisėse.**
    - Kai kuriais atvejais taikomoji programa gali būti trečioji šalis, tačiau ji gali būti registruota jūsų organizacijoje. Patikrinkite, ar ši taikomoji programa yra įtraukta į jūsų programų registracijas (ne įmonės taikomąsias programas).
    - Jei toliau matote šį klaidos pranešimą. Tada gali tekti sukurti sutikimo URL, aprašytą **4 veiksme.**
3. **Jei jūsų organizacija nėra taikomosios programos savininkas ir naudoja ją kaip trečiosios šalies taikomąją programą:**
    - Jei esate visuotinis / įmonės administratorius, turėtumėte matyti sutikimo ekraną. Įsitikinkite, kad pažymėkite žymės langelį **"Sutikimas organizacijos vardu".**
    - Jei nematote sutikimo ekrano, panaikinkite programą "Enterprise" ir bandykite dar kartą.
    - Jei toliau matote šį klaidos pranešimą. Tada gali tekti sukurti sutikimo URL, aprašytą **4 veiksme.**
4. **Neautomatiškai** sukurkite naudoti skirtą sutikimo URL: jei programa skirta pasiekti konkretų išteklių, gali būti, kad negalėsite naudoti mygtukų Sutikimas iš "Azure" portalo, turėsite rankiniu būdu sugeneruoti savo sutikimo URL ir jį naudoti.
    - Jums reikės gauti ir `{App-Id}` iš `{App-Uri-Id}` taikomosios programos savininko. `{Tenant-Id}` bus jūsų nuomotojo identifikatorius. Tai bus arba `yourdomain.onmicrosoft.com` jūsų katalogo ID.
    - Jei taikomoji programa pati turi prieigą prie ištekliaus, `{App-Id}` tada ir bus tokia `{App-Uri-Id}` pati.
5. Daugiau informacijos žr. Prisijungimo prie SAML pagrindu sukonfigūruotas bendrosios [afiksuojamų programų problemos.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Programų tinkinimas**

- Įtraukite prekės ženklo į savo organizacijos [""Azure Active Directory""](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) prisijungimo puslapį – naudokite organizacijos logotipą ir pasirinktines spalvų schemas, kad ""Azure Active Directory"" ("Azure AD") prisijungimo puslapiai būtų nuoseklūs.
- [Įtraukite savo pasirinktinį domeno vardą naudodami "Azure Active Directory" portalą](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – kiekvienas naujas "Azure AD" nuomotojas turi pradinį domeno vardą. Negalite keisti arba panaikinti pradinio domeno vardo, bet galite įtraukti savo organizacijos vardus. Pasirinktinių domenų vardų įtraukimas padeda kurti vartotojų vardus, kurie yra pažįstami jūsų vartotojams.
