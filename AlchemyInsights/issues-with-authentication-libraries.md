---
title: Autentifikavimo bibliotekų problemos
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028012"
---
# <a name="issues-with-authentication-libraries"></a>Autentifikavimo bibliotekų problemos

1. ["Microsoft" tapatybės platforma autentifikavimo bibliotekose išvardytos](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) "Microsoft" palaikomos ir suderinamos kliento ir programinės įrangos bibliotekos.
2. "Microsoft" autentifikavimo biblioteka (MSAL) palaiko kelis [autentifikavimo](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) srautus, kurie naudojami skirtinguose programų scenarijuose.
3. Norėdami autentifikuoti ir įsigyti atpažinimo ženklus, savo kode inicializuojate naują viešąją arba konfidencialią kliento taikomąją programą. Galite nustatyti kelias konfigūravimo parinktis, kai inicijuojate kliento programą "Microsoft" autentifikavimo bibliotekoje (MSAL). Norėdami sužinoti daugiau, [žr. Programos konfigūravimo parinktys](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**""Azure Active Directory"" autentifikavimo bibliotekos (ADAL) ir "Azure AD "Graph" API (AAD "Graph") palaikymo pabaiga**

**Nuo 2020 m. birželio 30** d. nebebus įtraukti naujų funkcijų į "ADAL" ir "Azure AD" "Graph". Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.

**Nuo 2022 m. birželio 30** d. baigsime "ADAL" ir "Azure AD "Graph"" palaikymą ir nebeteisime techninio palaikymo arba saugos naujinimų.

Programos, kurios naudoja ADAL esamoms OS versijoms, veiks po šio laiko, bet *negaus techninio palaikymo ar saugos naujinimų.*

Programos, kurios naudoja "Azure AD "Graph"" po šio laiko, gali nebegauti atsakymų iš "Azure AD" "Graph" pabaigos taško.

**ADAL perkėlimas**

Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.

Jei naudojate "Microsoft" programas, žinokite, kad "Microsoft" pereina prie MSAL iki palaikymo pabaigos termino, užtikrindama, kad jos gaus naudos iš MSAL vykdomų saugos ir funkcijų patobulinimų.

Daugiau informacijos rasite:

1. [Skaityti ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Sužinokite, kaip perkelti programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jei reikia pagalbos, kuri iš jūsų programų naudoja ADAL, rekomenduojame peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Programų, kurios naudoja "Azure AD "Graph"", vadovaukitės mūsų nurodymais, kaip perkelti ["Azure AD" "Graph" programas į "Microsoft "Graph"".](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Mūsų perkėlimo kontrolinis sąrašas pateikia darbo pradžios tašką.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. "Microsoft" palaikymas taip pat gali pateikti visų AAD "Graph" jūsų nuomotojo naudojimo sąrašą.
3. Kad jūsų programa turėtų prieigą prie "Microsoft "Graph"" duomenų, vartotojas arba administratorius turi suteikti reikiamas teises per sutikimo procesą. "Microsoft ["Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference) išvardytos teisės, susietos su kiekvienu svarbiu "Microsoft" "Graph" API. Jame taip pat pateikiama patarimų, kaip naudoti teises.
