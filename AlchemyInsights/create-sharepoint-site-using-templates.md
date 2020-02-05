---
title: Svetainės kūrimas SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770431"
---
# <a name="create-sharepoint-sites-using-templates"></a>"SharePoint" svetainių kūrimas naudojant šablonus

Galimybė įrašyti svetainę kaip šabloną nepalaiko šiuolaikinės bendravimo ar komandos svetainės. Daugiau informacijos apie šablonų naudojimą rasite [įrašyti, atsisiųsti ir nusiųsti "SharePoint" svetainę kaip šabloną](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Čia pateikiamos kelios Dažnos problemos/sprendimai dėl svetainės ar sąrašo įrašymo kaip "SharePoint Online" šablono. 

**Mygtukas įrašyti svetainės/sąrašo šabloną yra neprieinamas arba jo nėra**

Administratoriams reikės leisti pasirinktinį scenarijų, kad įgalintumėte šablono funkcijas. Išsamius veiksmus, pavyzdžius ir svarstymus žr. 

- [Leisti arba neleisti pasirinktinio scenarijaus](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda įrašyti svetainę kaip šabloną nepalaikoma ir gali sukelti problemų svetainėse, kurios naudoja SharePoint serverio publikavimo infrastruktūrą.

**Neįmanoma sukurti svetainės šablono arba tinkamai neveikti**

Šablone gali trūkti [funkcijos](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ir jos neaktyvinti. Jei šios funkcijos negalima aktyvinti dabartiniame svetainių rinkinyje, svetainės šablono negalite naudoti kurdami svetainę.

- Patikrinkite, ar sąrašai ir bibliotekos viršija 5000 elementų [sąrašo rodinio ribinę vertę](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , nes tai gali blokuoti svetainės šablono kūrimą.

- Svetainė gali naudoti per daug išteklių, todėl svetainės šablonas viršija 50 MB limitą.


- Yra problemų rodant duomenis iš sąrašo, kuris naudoja peržvalgos stulpelį. Daugiau informacijos ieškokite [šablono sugeneruotas sąraše nerodo duomenis iš tinkamą peržvalgos sąrašą SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Norėdami gauti išsamesnės informacijos apie bendrąsias problemas ir sprendimus, patikrinkite [kurti ir naudoti svetainės šablonus](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



