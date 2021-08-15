---
title: "\"Microsoft \"Graph\" API problemos"
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975901"
---
# <a name="microsoft-graph-api-issues"></a>"Microsoft "Graph" API problemos

Ši tema taip pat gali būti taikoma kūrėjams, vis dar naudojantys "Azure AD" "Graph" API. Tačiau primygtinai **rekomenduojama naudoti** "Microsoft "Graph" visus katalogus, tapatybę ir prieigos valdymo scenarijus.

**Autentifikavimo arba autorizavimo problemos**

- Jei jūsų programa **negali** įsigyti atpažinimo ženklų, kad paskambintų "Microsoft "Graph"", pasirinkite Problema gaunant prieigos **atpažinimo ženklą (autentifikavimą) "Microsoft** "Graph"" kategoriją, kad gautumėte daugiau konkrečios pagalbos ir palaikymo šia tema.
- Jei jūsų programa gauna **401 arba 403** autorizavimo klaidas, kai skambinate "Microsoft "Graph"", pasirinkite kategoriją Gauti prieigą **uždrausta (autorizuoti) "Microsoft** "Graph" API", kad gautumėte daugiau konkrečios pagalbos ir palaikymo šia tema.

**Noriu naudoti "Microsoft "Graph", bet nežinote, kur pradėti**

- ["Microsoft "Graph"](https://docs.microsoft.com/graph/overview)
- [Tapatybės ir "Access" valdymo "Microsoft "Graph"](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darbo pradžia kuriant "Microsoft "Graph"" programėles](https://docs.microsoft.com/graph/)
- **"Microsoft "Graph" Explorer"** – išbandykite "Microsoft "Graph" API savo nuomotojo arba demonstracinį nuomotoją

**Noriu naudoti "Microsoft "Graph", bet ar ji palaiko man reikalingas v1.0 katalogo API?**

"Microsoft "Graph"" yra rekomenduojama katalogo, tapatybės ir prieigos valdymo API. Tačiau vis dar yra keletas spragų tarp to, kas įmanoma "Azure AD "Graph" ir "Microsoft "Graph"". Peržiūrėkite šiuos straipsnius, kuriuose paryškinti naujausias skirtumai, padėsiintys pasirinkti:

- [Išteklių tipo skirtumai tarp "Azure AD" "Graph" "Microsoft "Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- ["Azure AD" ir "Microsoft "Graph"" ypatybių "Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- ["Azure AD" ir "Microsoft "Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, iš kurios skambinau, neveikia – kur galiu atlikti daugiau bandymų?**

**"Microsoft "Graph" Explorer"** – išbandykite "Microsoft "Graph"" API nuomotojo arba demonstracinio nuomotojo, taip pat peržiūrėkite užklausų **pavyzdžius** "Microsoft "Graph" Explorer".

**Mano programa yra per lėta ir taip pat yra suslėgta. Kokius patobulinimus galiu atlikti?**

Atsižvelgiant į scenarijų, jūsų žinioje yra įvairių parinkčių, kad jūsų taikomoji programa būtų efektyvesnė, o kai kuriais atvejais mažiau linkę į tai, kad tarnyba slegė (kai skambinate per daug skambučių).

- ["Microsoft "Graph" geriausia praktika](https://docs.microsoft.com/graph/best-practices-concept)
- [Paketinės užklausos](https://docs.microsoft.com/graph/json-batching)
- [Keitimų sekmas naudojant delta užklausą](https://docs.microsoft.com/graph/delta-query-overview)
- [Gauti pranešimus apie pakeitimus naudojant "webhooks"](https://docs.microsoft.com/graph/webhooks)
- [Throttling guidance](https://docs.microsoft.com/graph/throttling)

**Kur rasti daugiau informacijos apie klaidas ir žinomas problemas?**

- ["Microsoft "Graph"" atsakymo į klaidą informacija](https://docs.microsoft.com/graph/errors)
- [Žinomos "Microsoft "Graph"](https://docs.microsoft.com/graph/known-issues)

**Kur galiu patikrinti paslaugos pasiekiamumo ir ryšio būseną?**

Pagrindinių tarnybų, kurias galima pasiekti per "Microsoft "Graph"", pasiekiamumas ir ryšys gali turėti įtakos bendram "Microsoft "Graph"" pasiekiamumui ir "Graph".

- Jei "Azure Active Directory" tarnybos sveikatą, patikrinkite būseną **Sauga +** tapatybės tarnybos, nurodytos ["Azure" būsenos puslapyje.](https://azure.microsoft.com/status/)
- Jei Office prie "Microsoft "Graph"", patikrinkite tarnybų, išvardytų ["Office" tarnybos sveikatos ataskaitų srityje, būseną.](https://portal.office.com/adminportal/home#/servicehealth)

"Microsoft "Graph"" autorizavimo klaidos gali būti kelių skirtingų problemų, iš kurių dauguma generuoja 401 arba 403 klaidą, rezultatas. Pvz., dėl šių veiksmų gali kilti autorizavimo klaidų:

- Netinkami [atpažinimo ženklo gavimo srautai](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Prastai konfigūruotos [teisių aprėptys](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Sutikimo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkumas

***""Azure Active Directory"" autentifikavimo bibliotekos (ADAL) ir "Azure AD "Graph" API (AAD "Graph") palaikymo pabaiga***

**Nuo 2020 m. birželio 30** d. nebebus įtraukti naujų funkcijų į "ADAL" ir "Azure AD" "Graph". Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.

**Nuo 2022 m. birželio 30** d. baigsime "ADAL" ir "Azure AD "Graph"" palaikymą ir nebeteisime techninio palaikymo arba saugos naujinimų.

Programos, kurios naudoja ADAL esamoms OS versijoms, veiks po šio laiko, bet *negaus techninio palaikymo ar saugos naujinimų.*

Programos, kurios naudoja "Azure AD "Graph"" po šio laiko, gali nebegauti atsakymų iš "Azure AD" "Graph" pabaigos taško.

**ADAL perkėlimas**

Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.

Jei naudojate "Microsoft" programas, žinokite, kad "Microsoft" pereina prie MSAL iki palaikymo pabaigos termino, užtikrindama, kad jos naudos iš MSAL vykdomų saugos ir funkcijų patobulinimų.

1. [Skaityti ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Sužinokite, kaip perkelti programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jei reikia pagalbos, kuri iš jūsų programų naudoja ADAL, rekomenduojame peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Programų, kurios naudoja "Azure AD "Graph"", vadovaukitės mūsų nurodymais, kaip perkelti ["Azure AD" "Graph" programas į "Microsoft "Graph"".](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Mūsų perkėlimo kontroliniame sąraše apibūdinama darbo pradžia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. "Microsoft" palaikymas taip pat gali pateikti visų AAD "Graph" jūsų nuomotojo naudojimo sąrašą.
3. Kad jūsų programa turėtų prieigą prie "Microsoft "Graph"" duomenų, vartotojas arba administratorius turi suteikti reikiamas teises per sutikimo procesą. "Microsoft ["Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference) išvardytos teisės, susietos su kiekvienu svarbiu "Microsoft" "Graph" API. Jame taip pat pateikiama patarimų, kaip naudoti teises.
