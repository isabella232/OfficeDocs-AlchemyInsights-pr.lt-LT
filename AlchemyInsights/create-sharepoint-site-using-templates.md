---
title: Svetainės kūrimas "SharePoint Online"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732240"
---
# <a name="create-sharepoint-sites-using-templates"></a>"SharePoint" svetainių kūrimas naudojant šablonus

Galimybė įrašyti svetainę kaip šabloną nepalaikoma naudojant šiuolaikines ryšių arba komandos svetaines. Daugiau informacijos apie šablonų naudojimą rasite [įrašyti, atsisiųsti ir nusiųsti "SharePoint" svetainę kaip šabloną](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Štai keletas dažniausių problemų/sprendimų dėl svetainės arba sąrašo įrašymo kaip "SharePoint Online" šablono. 

**Nėra mygtuko įrašyti svetainės/sąrašo šablono arba jo nėra**

Administratoriams reikės leisti pasirinktiniam scenarijui įgalinti šablono funkcijas. Išsamių veiksmų, pavyzdžių ir aspektų žr. 

- [Pasirinktinio scenarijaus leidimas arba išvengimas](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda įrašyti svetainę kaip šabloną nepalaikoma, todėl gali kilti problemų svetainėse, naudojančioms "SharePoint Server" publikavimo infrastruktūrą.

**Negalima sukurti svetainės šablono arba jis veikia netinkamai**

Šablonui gali trūkti [funkcijos](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ir jis nebus suaktyvintas. Jei šios funkcijos negalima aktyvinti dabartiniame svetainių rinkinyje, svetainės šablono negalite naudoti svetainei sukurti.

- Patikrinkite, ar visi sąrašai ir bibliotekos viršija 5000 elementų [sąrašo rodinio limito ribą](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , nes tai gali blokuoti svetainės šablono sukūrimą.

- Svetainė gali naudoti per daug išteklių, todėl svetainės šablonas viršija 50 MB ribą.


- Kyla problemų rodant duomenis iš sąrašo, kuris naudoja peržvalgos stulpelį. Daugiau informacijos ieškokite [šablono sugeneruotas sąrašas nerodo duomenų iš tinkamo peržvalgos sąrašo "SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)".

Išsamesnės informacijos apie įprastas problemas ir sprendimus ieškokite [svetainės šablonų kūrimas ir naudojimas](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



