---
title: Problemos kuriant taikomąsias programas su API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974623"
---
# <a name="issues-developing-applications-with-apis"></a>Problemos kuriant taikomąsias programas su API

Norėdami pradėti naudoti "Azure Active Directory Graph" API, peržiūrėkite " [AZURE ad GRAPH API" greitojo pasirengimo darbui vadovą](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) arba peržiūrėkite [INTERAKTYVIĄ "Azure AD Graph" API nuorodų dokumentaciją](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**"Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "Azure AD Graph" API (AAD Graph) palaikymo nutraukimas**

**Nuo birželio 30 d., 2020**, mes nebeįtrauksime jokių naujų "adal" ir "Azure AD Graph" funkcijų. Mes ir toliau suteiksime techninio palaikymo ir saugos naujinimus, tačiau nebepateiksime funkcijų naujinimų.

**Nuo birželio 30 d., 2022**, mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.

Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės gauti jokio techninio palaikymo ar saugos naujinimų.

Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.

**ADAL perkėlimas**

Rekomenduojame naujinti į ["Microsoft" autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kuri turi naujausias funkcijas ir saugos naujinimus.

Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft" proceso metu migruoja jo taikomąsias programas į "MSAL" iki palaikymo termino pabaigos ir užtikrins, kad jos bus naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.

1. [Perskaitykite ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Sužinokite, kaip perkelti taikomąsias programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Jei reikia pagalbos norint suprasti, kurios iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriuo ISVs arba taikomųjų programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti jums visų ne "Microsoft" ADAL taikomųjų programų sąrašą savo nuomotojuje.

**AAD Graph perkėlimas**

Jei naudojate "Azure AD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip perkelti ["AZURE ad Graph" taikomąsias programas į "Microsoft Graph"](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. "Azure App" registracijos portale rodoma, kurios taikomosios programos naudoja AAD grafiką. Rekomenduojame Peržiūrėti visus savo taikomųjų programų šaltinio kodus ir, jei reikia, pasiekti bet kokius ISVs arba taikomųjų programų teikėjus. "Microsoft" palaikymas taip pat gali suteikti jums sąrašą visų "AAD Graph" naudojimo jūsų nuomotojuje.
1. Jei norite, kad programa pasiektų duomenis programoje "Microsoft Graph", vartotojas arba administratorius, naudodamas sutikimo procesą, privalo suteikti jam teisingas teises. ["Microsoft Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) išvardijamos teisės, susietos su kiekvienu pagrindiniu "Microsoft Graph" API rinkiniu. Taip pat pateikiama rekomendacijų, kaip naudoti teises.
