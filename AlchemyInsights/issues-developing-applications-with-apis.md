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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013468"
---
# <a name="issues-developing-applications-with-apis"></a>Problemos kuriant taikomąsias programas su API

Norėdami pradėti naudoti "Azure Active Directory" "Graph" API, žr. ["Azure AD "Graph" API"](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) greito pasirengimo darbui vadovą arba peržiūrėkite interaktyvią ["Azure AD" "Graph" API nuorodos dokumentaciją.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**""Azure Active Directory"" autentifikavimo bibliotekos (ADAL) ir "Azure AD "Graph" API (AAD "Graph") palaikymo pabaiga**

**Nuo 2020 m. birželio 30** d. nebebus įtraukti naujų funkcijų į "ADAL" ir "Azure AD" "Graph". Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.

**Nuo 2022 m. birželio 30** d. baigsime "ADAL" ir "Azure AD "Graph"" palaikymą ir nebeteisime techninio palaikymo arba saugos naujinimų.

Programos, kurios naudoja ADAL esamoms OS versijoms, po šio laiko veiks ir toliau, tačiau negaus jokių techninio palaikymo ar saugos naujinimų.

Programos, kurios naudoja "Azure AD "Graph"" po šio laiko, gali nebegauti atsakymų iš "Azure AD" "Graph" pabaigos taško.

**ADAL perkėlimas**

Rekomenduojame atnaujinti į [„Microsoft“ autentifikavimo biblioteką (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurioje yra naujausios funkcijos ir saugos naujinimai.

Jei naudojate "Microsoft" programas, žinokite, kad "Microsoft" šiuo metu perkelia savo taikomąsias programas į MSAL iki galutinio palaikymo termino, užtikrindama, kad jos naudos iš MSAL vykdomų saugos ir funkcijų patobulinimų.

1. [Skaitykite ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Sužinokite, kaip perkelti programas per platformą.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Jei reikia pagalbos, kuri iš jūsų programų naudoja ADAL, rekomenduojame peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Jei naudojate "Azure AD "Graph"", vadovaukitės mūsų nurodymais, kaip perkelti ["Azure AD "Graph"" programas į "Microsoft "Graph"".](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Mūsų perkėlimo kontroliniame sąraše apibūdinama darbo pradžia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visą programų šaltinio kodą ir, jei taikoma, susisiekti su visais ISV arba programų teikėjais. "Microsoft" palaikymas taip pat gali pateikti visų AAD "Graph" jūsų nuomotojo naudojimo sąrašą.
1. Kad jūsų programa turėtų prieigą prie "Microsoft "Graph"" duomenų, vartotojas arba administratorius turi suteikti reikiamas teises per sutikimo procesą. "Microsoft ["Graph" teisių nuorodoje](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) išvardytos teisės, susietos su kiekvienu svarbiu "Microsoft" "Graph" API. Jame taip pat pateikiama patarimų, kaip naudoti teises.
