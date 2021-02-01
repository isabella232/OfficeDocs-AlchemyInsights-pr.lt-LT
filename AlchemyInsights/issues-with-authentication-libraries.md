---
title: Problemos su autentifikavimo bibliotekomis
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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063638"
---
# <a name="issues-with-authentication-libraries"></a>Problemos su autentifikavimo bibliotekomis

1. ["Microsoft" tapatybės platformos autentifikavimo bibliotekose](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) pateikiami "Microsoft" palaikomi ir suderinami kliento ir "tarpinės" bibliotekos.
2. "Microsoft" autentifikavimo biblioteka (MSAL) palaiko kelis [autentifikavimo srautus](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) , skirtus naudoti skirtinguose taikomosios programos scenarijuose.
3. Norėdami autentifikuoti ir įsigyti atpažinimo ženklus, inicijuokite savo kode naują viešą arba konfidencialią kliento taikomąją programą. Galite nustatyti kelias konfigūravimo parinktis, kai inicijuojate kliento programą "Microsoft" autentifikavimo bibliotekoje (MSAL). Norėdami sužinoti daugiau, peržiūrėkite [taikomosios programos konfigūravimo parinktys](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**"Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "Azure AD Graph" API (AAD Graph) palaikymo nutraukimas**

**Nuo birželio 30 d., 2020**, mes nebeįtrauksime jokių naujų "adal" ir "Azure AD Graph" funkcijų. Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.

**Nuo birželio 30 d., 2022**, mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.

Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės *gauti jokio techninio palaikymo ar saugos naujinimų*.

Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.

**ADAL perkėlimas**

Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.

Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft" proceso metu migruoja jo taikomąsias programas į "MSAL" iki palaikymo termino pabaigos ir užtikrins, kad bus naudingi "MSAL" saugos ir funkcijų patobulinimai.

Daugiau informacijos rasite:

1. [Skaityti ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Sužinokite, kaip perkelti programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo ISVs arba taikomųjų programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Jei naudojate "Azure AD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip [perkelti "AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti jums sąrašą visų "AAD Graph" naudojimo jūsų nuomotojuje.
3. Jei norite, kad programa pasiektų duomenis programoje "Microsoft Graph", vartotojas arba administratorius, naudodamas sutikimo procesą, privalo suteikti jam teisingas teises. ["Microsoft Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference) išvardijamos teisės, susietos su kiekvienu pagrindiniu "Microsoft Graph" API rinkiniu. Taip pat pateikiama rekomendacijų, kaip naudoti teises.
