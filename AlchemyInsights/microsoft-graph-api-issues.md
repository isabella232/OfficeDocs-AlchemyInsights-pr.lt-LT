---
title: "\"Microsoft Graph\" API problemos"
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714153"
---
# <a name="microsoft-graph-api-issues"></a>"Microsoft Graph" API problemos

Ši tema taip pat gali būti taikoma kūrėjams, kurie vis dar naudoja "Azure AD Graph API". Tačiau **primygtinai** rekomenduojama naudoti "Microsoft Graph" visiems jūsų katalogo, tapatybės ir "Access" valdymo scenarijams.

**Autentifikavimo arba autorizavimo problemos**

- Jei jūsų programai **nepavyksta įsigyti žetonų** norint paskambinti "Microsoft Graph", pasirinkite problemą, kad gautumėte " **Access" atpažinimo ženklo (autentifikavimo)** "Microsoft Graph" kategoriją, kad gautumėte daugiau konkrečios žinyno ir palaikymo šioje temoje.
- Jei jūsų programa **gauna "401" arba "403" autorizavimo klaidas** , kai skambinate "Microsoft Graph", pasirinkite "Microsoft Graph API" kategoriją gauti prieigą prie " **Access Denied" (leidimas)** , kad šioje temoje gautumėte konkretesnį žinyną ir palaikymą.

**Noriu naudoti "Microsoft Graph", bet nežinote, nuo ko pradėti**

- ["Microsoft Graph" apžvalga](https://docs.microsoft.com/graph/overview)
- [Tapatybės ir "Access" valdymo apžvalga programoje "Microsoft Graph"](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darbo pradžia "Microsoft Graph" taikomųjų programų kūrimas](https://docs.microsoft.com/graph/)
- **"Microsoft Graph Explorer"** – jūsų nuomotojo arba demonstracinio kompiuterio "Microsoft Graph" API bandymas

**Noriu naudoti "Microsoft Graph", tačiau ar ji palaiko "v 1.0" katalogo API, kurių man reikia?**

"Microsoft Graph" yra rekomenduojamas katalogo, tapatybės ir "Access" valdymo API. Tačiau vis dar yra kelios spragos tarp to, kas įmanoma, "Azure AD Graph" ir "Microsoft Graph". Peržiūrėkite šiuos straipsnius, kuriuose Akcentuokite naujausius skirtumus, kurie padės jums pasirinkti:

- [Išteklių tipo skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Ypatybių skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- ["Azure AD" ir "Microsoft Graph" metodo skirtumai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Mano skambinimo API neveikia – kur galiu atlikti daugiau bandymų?**

**"Microsoft Graph Explorer"** – Išbandykite "Microsoft Graph" API savo nuomotojuje arba "demo" nuomotojuje, taip pat peržiūrėkite **užklausų užklausas** programoje "Microsoft Graph Explorer".

**Mano programa yra per lėta ir taip pat yra Throttled. Kokius patobulinimus galiu padaryti?**

Atsižvelgiant į jūsų scenarijų, jūsų dispozicijoje yra įvairių parinkčių, kad jūsų programa būtų efektyvesnė, o kai kuriais atvejais, mažiau linkę ją naudoti (kai skambinate per daug kartų).

- ["Microsoft Graph" geriausios praktikos](https://docs.microsoft.com/graph/best-practices-concept)
- [Užklausų grupavimas](https://docs.microsoft.com/graph/json-batching)
- [Keitimų sekimas naudojant Delta užklausą](https://docs.microsoft.com/graph/delta-query-overview)
- [Gaukite pranešimus apie keitimą naudodami webkablius](https://docs.microsoft.com/graph/webhooks)
- [Ribojimo gairės](https://docs.microsoft.com/graph/throttling)

**Kur galiu gauti daugiau informacijos apie klaidas ir žinomas problemas?**

- ["Microsoft Graph" klaidos atsakymo informacija](https://docs.microsoft.com/graph/errors)
- [Žinomos "Microsoft Graph" problemos](https://docs.microsoft.com/graph/known-issues)

**Kur galiu patikrinti paslaugų pasiekiamumo ir ryšio būseną?**

Tarnybų pasiekiamumo ir ryšio su pagrindinėmis tarnybomis, kurias galima pasiekti naudojant "Microsoft Graph", paslaugos gali turėti įtakos bendram "Microsoft Graph" pasiekiamumui ir veikimui.

- "Azure Active Directory" tarnybos sveikatai patikrinkite **saugos + tapatybės** tarnybų būseną, išvardytas "Azure" [būsenos puslapyje](https://azure.microsoft.com/status/).
- "Office" tarnyboms, kurios prisideda prie "Microsoft Graph", patikrinkite tarnybų, išvardintų " [Office" tarnybos sveikatos ataskaitų](https://portal.office.com/adminportal/home#/servicehealth)srityje, būseną.

"Microsoft Graph" autorizavimo klaidos gali kilti dėl kelių skirtingų problemų, kurių dauguma generuoja "401" arba "403" klaidą. Pavyzdžiui, toliau nurodyti būdai gali sukelti autorizavimo klaidas:

- Netinkami [atpažinimo ženklo gavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Prastai konfigūruotos [teisių aprėptys](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkumas

**_„Azure Active Directory“ autentifikavimo bibliotekos (ADAL) ir „Azure AD Graph“ API („AAD Graph“) palaikymo pabaiga_* _

* Nuo birželio 30 d., 2020 * *, mes nebeįtrauksime jokių naujų funkcijų į ADAL ir Azure AD Graph. Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.

**Nuo birželio 30 d., 2022**, mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.

Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės *gauti jokio techninio palaikymo ar saugos naujinimų*.

Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.

**ADAL perkėlimas**

Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.

Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft" proceso metu migruoja jo taikomąsias programas į "MSAL" iki palaikymo termino pabaigos ir užtikrins, kad jos bus naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.

1. [Skaityti ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Sužinokite, kaip perkelti programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo ISVs arba taikomųjų programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Jei naudojate "Azure AD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip [perkelti "AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Mūsų perkėlimo kontroliniame sąraše apibūdinama darbo pradžia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti jums sąrašą visų "AAD Graph" naudojimo jūsų nuomotojuje.
3. Jei norite, kad programa pasiektų duomenis programoje "Microsoft Graph", vartotojas arba administratorius, naudodamas sutikimo procesą, privalo suteikti jam teisingas teises. ["Microsoft Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference) išvardijamos teisės, susietos su kiekvienu pagrindiniu "Microsoft Graph" API rinkiniu. Taip pat pateikiama rekomendacijų, kaip naudoti teises.
