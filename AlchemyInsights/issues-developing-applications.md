---
title: Programų kūrimo problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013432"
---
# <a name="issues-developing-applications"></a>Programų kūrimo problemos

Norėdami šalinti dažniausiai pasitaikančių ""Azure Active Directory" (AD) programų triktis, žr. šiuos straipsnius:

- [Matau problemų prisijungiant prie taikomosios (-ių) programos (-ų) naudojant tik "Chrome" naršyklę](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nežinau, kaip pakeisti atpažinimo ženklo naudojimo trukmės numatytąsias reikšmes mano programoje](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Esu paini apie tai, kaip veikia programos sutikimas](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nežinau, kaip suteikti teises savo programai](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nesuprantu skirtumo tarp įgaliotųjų ir taikomųjų programų teisių](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***""Azure Active Directory"" autentifikavimo bibliotekos (ADAL) ir "Azure AD "Graph" API (AAD "Graph") palaikymo pabaiga***

- Nuo 2020 m. birželio 30 d. mes neįtrauksime jokių naujų funkcijų į „Azure Active Directory“ autentifikavimo biblioteką (ADAL) ir „Azure AD Graph“ API („AAD Graph“). Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.

- Nuo 2022 m. birželio 30 d. baigsime ADAL ir „AAD Graph“ palaikymą ir nebeteisime techninio palaikymo ar saugos naujinimų. Dėl šios sąlygos pasekmės yra šios:

    - Programos, kurios naudoja ADAL esamoms OS versijoms, po šio laiko veiks ir toliau, tačiau negaus jokių techninio palaikymo ar saugos naujinimų.

    - Programos, kurios "Graph" AAD, gali nebegauti atsakymų iš AAD "Graph" pabaigos taško

**ADAL perkėlimas**

Jei naudojate "Microsoft" programas, rekomenduojame atnaujinti į "Microsoft" autentifikavimo biblioteką (MSAL), kurioje yra naujausių funkcijų ir saugos naujinimų. Ši rekomendacija pateikta atsižvelgiant į tai, kad "Microsoft" inicijuoja savo programų perkėlimo į MSAL procesą iki palaikymo pabaigos termino. 

"Microsoft" perkėlus savo programėles į MSAL užtikrinama, kad programos naudos iš MSAL vykdomų saugos ir funkcijų patobulinimų.

1. [Skaityti ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Sužinokite, kaip perkelti programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jei reikia pagalbos, kad suprastumėte, kurios iš jūsų programų naudoja ADAL, rekomenduojame peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su nepriklausomais programinės įrangos tiekėjais (ISV) arba programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.

**„AAD Graph“ perkėlimas**

Taikomųjų programų, kurios naudoja AAD "Graph", vadovaukitės mūsų nurodymais, kaip perkelti AAD "Graph" programas į "Microsoft "Graph"":

1. [Mūsų perkėlimo kontroliniame sąraše apibūdinama darbo pradžia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Jūsų „Azure“ programos registracijos portale rodoma, kuriose programose naudojama „AAD Graph“. Rekomenduojame peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su nepriklausomais programinės įrangos tiekėjais (ISV) arba programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti informacijos apie AAD "Graph" jūsų nuomotojo naudojimą.







