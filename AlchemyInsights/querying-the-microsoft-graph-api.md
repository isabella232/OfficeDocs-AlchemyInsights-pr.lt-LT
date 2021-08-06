---
title: "\"Microsoft \"Graph\" API užklausa"
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923247"
---
# <a name="querying-the-microsoft-graph-api"></a>"Microsoft "Graph" API užklausa

Ši tema taip pat gali būti taikoma kūrėjams, vis dar naudojantys "Azure AD" "Graph" API. Tačiau primygtinai **rekomenduojama naudoti** "Microsoft "Graph" visus katalogus, tapatybę ir prieigos valdymo scenarijus.

**Autentifikavimo arba autorizavimo problemos**

- Jei jūsų programa **negali** įsigyti atpažinimo ženklų, kad paskambintų "Microsoft "Graph"", pasirinkite Problema gaunant prieigos **atpažinimo ženklą (autentifikavimą) "Microsoft** "Graph"" kategoriją, kad gautumėte daugiau konkrečios pagalbos ir palaikymo šia tema.
- Jei jūsų programa gauna **401 arba 403** autorizavimo klaidas, kai skambinate "Microsoft "Graph"", pasirinkite kategoriją Gauti prieigą **uždrausta (autorizuoti) "Microsoft** "Graph" API", kad gautumėte daugiau konkrečios pagalbos ir palaikymo šia tema.

**Noriu naudoti "Microsoft "Graph", bet nežinote, kur pradėti**

Norėdami sužinoti daugiau apie "Microsoft "Graph", žr.:

- ["Microsoft "Graph"](https://docs.microsoft.com/graph/overview)
- [Tapatybės ir "Access" valdymo "Microsoft "Graph"](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darbo pradžia kuriant "Microsoft "Graph"" programėles](https://docs.microsoft.com/graph/)
- **"Microsoft "Graph" Explorer"** – išbandykite "Microsoft "Graph" API savo nuomotojo arba demonstracinį nuomotoją

**Noriu naudoti "Microsoft "Graph", bet ar ji palaiko man reikalingas v1.0 katalogo API?**

"Microsoft "Graph"" yra rekomenduojama katalogo, tapatybės ir prieigos valdymo API. Tačiau vis dar yra keletas spragų tarp to, kas įmanoma "Azure AD "Graph" ir "Microsoft "Graph"". Peržiūrėkite šiuos straipsnius, kuriuose paryškinti naujausias skirtumai, padėsiintys pasirinkti:

- [Išteklių tipo skirtumai tarp "Azure AD" "Graph" "Microsoft "Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- ["Azure AD" ir "Microsoft "Graph"" ypatybių "Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- ["Azure AD" ir "Microsoft "Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kai pateikiau vartotojo *objekto užklausą,* trūksta daugelio jo savybių**

`GET https://graph.microsoft.com/v1.0/users`grąžina tik 11 ypatybes, nes "Microsoft "Graph" automatiškai pasirenka numatytąjį grąžinti *vartotojo* savybių rinkinį. Jei jums reikia kitų *vartotojo* ypatybės, $select pasirinkite ypatybes, reikalingas jūsų programai. Pirmiausia išbandykite ją **"Microsoft "Graph" Explorer".**

**Kai kurios vartotojo ypatybių reikšmės yra *neapibrėžtos,* nors žinau, kad jos nustatytos**

Labiausiai tikėtina, kad programai buvo suteiktos *User.ReadBasic.All* teisės. Tai leidžia programai skaityti ribotą vartotojų savybių rinkinį, grąžinant visas kitas ypatybes kaip neapibrėžtas, net jei jos anksčiau buvo nustatytos. Pabandykite suteikti taikomosios programos *User.Read.All* teises.

Daugiau informacijos žr. ["Microsoft "Graph" vartotojo teisės](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Kyla problemų naudojant "OData" užklausos parametrus užklausų duomenims filtruoti**

Nors "Microsoft "Graph"" palaiko platų "OData" užklausos parametrų diapazoną, daugelis šių parametrų nevisiškai palaikomi katalogų tarnybos (ištekliai, paveldimi iš *directoryObject)*"Microsoft "Graph"". Tie patys apribojimai, kurie buvo pateikti "Azure AD"Graph" išlieka daugiausia "Microsoft "Graph"":

1. **Nepalaikoma:**$count, $search ir $filter *reikšmės* null arba *ne null*
2. **Nepalaikoma**: $filter ypatybes (žr. išteklių temas, kuriose galima filtruoti ypatybes)
3. **Nepalaikoma:** puslapių ėjimas, filtravimas ir rūšiavimas vienu metu
4. **Nepalaikoma**: ryšio filtravimas. Pvz., raskite visus jungtinės karalystės inžinierių grupės narius.
5. **Dalinis** palaikymas: $orderby *(tik* "displayName" ir "userPrincipalName") ir *grupės*
6. **Dalinis** palaikymas: "$filter" (palaiko tik *eq* *,* *startswith* arba , *ir*, ir , ir tik *bet* kurį ) palaikymą, "$expand" (išplečiant vieno objekto ryšius grąžina visus ryšius, bet objektų ryšių rinkinio išplėtimas yra ribotas)

Daugiau informacijos žr. [Atsakymų tinkinimas naudojant užklausos parametrus](https://docs.microsoft.com/graph/query-parameters).

**Neveikia API, iš kurios skambinau – kur galiu atlikti daugiau bandymų?**

**"Microsoft "Graph" Explorer"** – išbandykite "Microsoft "Graph"" API nuomotojo arba demonstracinio nuomotojo, taip pat peržiūrėkite užklausų **pavyzdžius** "Microsoft "Graph" Explorer".

**Kai pateikiau užklausą dėl duomenų, atrodo, kad vėl gaunu nebaigtą duomenų rinkinį**

Jei pateikiate užklausą rinkiniui (pvz., *vartotojams),*"Microsoft "Graph"" naudoja serverio puslapio apribojimus, todėl rezultatai visada pateikiami su numatytuoju puslapio dydžiu. Jūsų programa turėtų visada tikėtis puslapių per rinkinius, grąžintų iš tarnybos.

Daugiau informacijos rasite:

- ["Microsoft "Graph" geriausia praktika](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft "Graph" data in your app](https://docs.microsoft.com/graph/paging)

**Mano programa yra per lėta ir taip pat yra suslėgta. Kokius patobulinimus galiu atlikti?**

Atsižvelgiant į scenarijų, jūsų žinioje yra įvairių skirtingų parinkčių, kad jūsų taikomoji programa būtų efektyvesnė, o kai kuriais atvejais – mažiau linkę į tai, kad tarnyba slegė (kai skambinate per daug skambučių).

Jei norite sužinoti daugiau, žr.:

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
