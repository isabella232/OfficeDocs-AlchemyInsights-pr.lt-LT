---
title: "\"Microsoft Graph\" API užklausų užklausa"
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974423"
---
# <a name="querying-the-microsoft-graph-api"></a>"Microsoft Graph" API užklausų užklausa

Ši tema taip pat gali būti taikoma kūrėjams, kurie vis dar naudoja "Azure AD Graph API". Tačiau **primygtinai** rekomenduojama naudoti "Microsoft Graph" visiems jūsų katalogo, tapatybės ir "Access" valdymo scenarijams.

**Autentifikavimo arba autorizavimo problemos**

- Jei jūsų programai **nepavyksta įsigyti žetonų** norint paskambinti "Microsoft Graph", pasirinkite problemą, kad gautumėte " **Access" atpažinimo ženklo (autentifikavimo)** "Microsoft Graph" kategoriją, kad gautumėte daugiau konkrečios žinyno ir palaikymo šioje temoje.
- Jei jūsų programa **gauna "401" arba "403" autorizavimo klaidas** , kai skambinate "Microsoft Graph", pasirinkite "Microsoft Graph API" kategoriją gauti prieigą prie " **Access Denied" (leidimas)** , kad šioje temoje gautumėte konkretesnį žinyną ir palaikymą.

**Noriu naudoti "Microsoft Graph", bet nežinote, nuo ko pradėti**

Norėdami sužinoti daugiau apie "Microsoft Graph", žiūrėkite:

- ["Microsoft Graph" apžvalga](https://docs.microsoft.com/graph/overview)
- [Tapatybės ir "Access" valdymo apžvalga programoje "Microsoft Graph"](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darbo pradžia "Microsoft Graph" taikomųjų programų kūrimas](https://docs.microsoft.com/graph/)
- **"Microsoft Graph Explorer"** – jūsų nuomotojo arba demonstracinio kompiuterio "Microsoft Graph" API bandymas

**Noriu naudoti "Microsoft Graph", tačiau ar ji palaiko "v 1.0" katalogo API, kurių man reikia?**

"Microsoft Graph" yra rekomenduojamas katalogo, tapatybės ir "Access" valdymo API. Tačiau vis dar yra kelios spragos tarp to, kas įmanoma, "Azure AD Graph" ir "Microsoft Graph". Peržiūrėkite šiuos straipsnius, kuriuose Akcentuokite naujausius skirtumus, kurie padės jums pasirinkti:

- [Išteklių tipo skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Ypatybių skirtumai tarp "Azure AD Graph" ir "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- ["Azure AD" ir "Microsoft Graph" metodo skirtumai](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kai gaunu užklausą dėl *vartotojo* objekto, daugelis jo ypatybių nėra**

`GET https://graph.microsoft.com/v1.0/users` pateikia tik 11 ypatybių, nes "Microsoft Graph" automatiškai parenka numatytąjį *vartotojų* ypatybių rinkinį. Jei reikia kitų *vartotojo* ypatybių, naudokite $Select, kad pasirinktumėte programos poreikius. Išbandykite **"Microsoft Graph Explorer"** pirmiausia.

**Kai kurios vartotojo ypatybių reikšmės yra *NULL* , nors žinau, kad jos nustatytos**

Greičiausiai paaiškinimas yra tas, kad taikomajai programai buvo suteiktas *vartotojas. ReadBasic. All* Permission. Tai leidžia programai skaityti ribotą vartotojų ypatybių rinkinį, grąžinant visas kitas ypatybes kaip NULL, net jei jos buvo anksčiau nustatytos. Bandykite suteikti taikomosios programos *vartotoją. skaityti. visi* teisės.

Daugiau informacijos ieškokite ["Microsoft Graph" vartotojų teisės](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Kyla problemų naudojant "OData" užklausos parametrus duomenims filtruoti pagal savo užklausas**

Nors "Microsoft Graph" palaiko platų "OData" užklausos parametrų intervalą, daugelis šių parametrų katalogų tarnybos nevisiškai palaiko (ištekliai, kurie paveldimi iš *Directoryobject*) programoje "Microsoft Graph". Tie patys apribojimai, kurie buvo pateikti "Azure AD Graph", išlieka daugiausia programoje "Microsoft Graph":

1. **Nepalaikoma: $Count**, $search ir $Filter *NULL* arba *Not Null* reikšmės
2. **Nepalaikoma: $Filter** tam tikrų ypatybių (Peržiūrėkite išteklių temas, kuriose yra filtruojami ypatybės)
3. **Nepalaikoma: puslapių** kaita, filtravimas ir rūšiavimas vienu metu
4. **Nepalaikoma: ryšio** filtravimas. Pavyzdžiui – raskite visus Jungtinės Karalystės inžinerijos grupės narius.
5. **Dalinis palaikymas**: $OrderBy *vartotojui* (tik DisplayName ir UserPrincipalName) ir *grupėje*
6. **Dalinis palaikymas**: $Filter (palaiko tik *EQ*, *Startswith*, *or* ir *and* *ir Limited)* palaikymą, $Expand (vieno objekto ryšių išplėtimas grąžina visus ryšius, bet objektų ryšių rinkinio išplėtimas yra ribotas)

Daugiau informacijos ieškokite [atsakymų su užklausos parametrais tinkinimas](https://docs.microsoft.com/graph/query-parameters).

**Mano skambinimo API neveikia – kur galiu atlikti daugiau bandymų?**

**"Microsoft Graph Explorer"** – Išbandykite "Microsoft Graph" API savo nuomotojuje arba "demo" nuomotojuje, taip pat peržiūrėkite **užklausų užklausas** programoje "Microsoft Graph Explorer".

**Kai gaunu užklausą dėl duomenų, atrodo, kad gaunu neišsamią duomenų rinkinį**

Jei užklausiate rinkinį (pvz., *vartotojai*), "Microsoft Graph" naudoja serverio pusės puslapio apribojimus, todėl rezultatai visada grąžinami su numatytuoju puslapio dydžiu. Jūsų programa visada turėtų tikėtis puslapio iš tarnybos grąžintų rinkinių.

Daugiau informacijos rasite:

- ["Microsoft Graph" geriausios praktikos](https://docs.microsoft.com/graph/best-practices-concept)
- ["Microsoft Graph" duomenų puslapių ieška taikomojoje programoje](https://docs.microsoft.com/graph/paging)

**Mano programa yra per lėta ir taip pat yra Throttled. Kokius patobulinimus galiu padaryti?**

Atsižvelgiant į jūsų scenarijų, jūsų dispozicijoje yra įvairių įvairių parinkčių, kad jūsų programa būtų efektyvesnė, o kai kuriais atvejais mažiau būtų sulaikoma tarnyba (kai skambinate per daug kartų).

Jei norite sužinoti daugiau, žr.:

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
