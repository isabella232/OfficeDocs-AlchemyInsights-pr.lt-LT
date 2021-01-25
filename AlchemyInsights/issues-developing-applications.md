---
title: Problemos kuriant taikomąsias programas
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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974470"
---
# <a name="issues-developing-applications"></a>Problemos kuriant taikomąsias programas

Norėdami pašalinti Dažniausias "Azure Active Directory" (AD) programų kūrimo problemas, skaitykite šiuos straipsnius:

- [Matau problemų prisijungiant prie taikomosios programos (-ų) naudojant tik "Chrome" naršyklę](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Nežinau, kaip pakeisti atpažinimo ženklo naudojimo numatytuosius parametrus mano taikomojoje programoje](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Aš painiojama apie tai, kaip veikia taikomųjų programų sutikimas](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Nežinau, kaip suteikti teises savo taikomajai programai](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nesuprantu skirtumo tarp įgaliotųjų ir taikomosios programos teisių](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

*" **Azure Active Directory" autentifikavimo bibliotekos (ADAL) ir "AZURE ad Graph" API (AAD grafikas) palaikymo pabaiga**

- Nuo birželio 30 d., 2020, nebegalėsime įtraukti jokių naujų funkcijų į "Azure Active Directory" autentifikavimo biblioteką (ADAL) ir "Azure AD Graph API" (AAD Graph). Mes ir toliau suteiksime techninio palaikymo ir saugos naujinimus, tačiau nebepateiksime funkcijų naujinimų.

- Nuo birželio 30 d., 2022, mes užbaigsime ADAL ir AAD Graph palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų. Dėl šios sąlygos, toliau pateikiami padariniai:

    - Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės gauti jokio techninio palaikymo ar saugos naujinimų.

    - Taikomosios programos, naudojančios AAD grafiką po šio laiko, gali nebegauti atsakymų iš AAD diagramos galinio punkto

−*Adal perkėlimas**

Jei naudojate "Microsoft" taikomąsias programas, rekomenduojame naujinti į "Microsoft" autentifikavimo biblioteką (MSAL), kuri turi naujausias funkcijas ir saugos naujinimus. Ši rekomendacija parengta atsižvelgiant į tai, kad "Microsoft" pradeda perkelti savo taikomąsias programas į MSAL iki palaikymo termino pabaigos. 

"Microsoft" vykdomas "Microsoft" perkėlimas į "MSAL" užtikrina, kad taikomosios programos naudos iš MSAL vykstančių saugos ir funkcijų patobulinimų.

1. [DUK apie ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Sužinokite, kaip perkelti taikomąsias programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Jei jums reikia pagalbos suprasti, kurią iš jūsų taikomųjų programų naudoja ADAL, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus ir, jei taikoma, susisiekti su bet kuriuo nepriklausomu programinės įrangos pardavėjais (ISVs) arba taikomųjų programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti jums visų ne "Microsoft" ADAL taikomųjų programų sąrašą savo nuomotojuje.

**AAD Graph perkėlimas**

Jei naudojate "AAD Graph" taikomąsias programas, vadovaukitės mūsų rekomendacijomis, kaip perkelti "AAD Graph" taikomąsias programas į "Microsoft Graph":

1. [Mūsų perkėlimo kontrolinis sąrašas suteikia darbo pradžios tašką](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. "Azure App" registracijos portale rodoma, kurios taikomosios programos naudoja AAD grafiką. Rekomenduojame Peržiūrėti visus savo taikomųjų programų šaltinio kodus ir, jei reikia, susisiekti su bet kuriais nepriklausomais programinės įrangos tiekėjais (ISVs) arba taikomųjų programų teikėjais. "Microsoft" palaikymas taip pat gali suteikti informacijos apie "AAD Graph" naudojimą jūsų nuomotojuje.







