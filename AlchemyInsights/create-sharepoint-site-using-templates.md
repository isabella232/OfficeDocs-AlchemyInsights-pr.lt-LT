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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057974"
---
# <a name="create-sharepoint-sites-using-templates"></a>Svetainių SharePoint naudojant šablonus

Galimybė įrašyti svetainę kaip šabloną nepalaikoma naudojant šiuolaikiškas bendravimo arba komandos svetaines. Daugiau informacijos apie šablonų naudojimo žr. Svetainės kaip šablono [SharePoint, atsisiuntimas ir nusiuntimas.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Štai keletas dažnai pasitaikančių problemų / sprendimų, susijusių su svetainės arba sąrašo įrašymą kaip šabloną "Sharepoint Online". 

**Mygtukas Įrašyti svetainės / sąrašo šabloną negalimas arba jo nėra**

Administratoriai turės leisti pasirinktinį scenarijų, kad įgalintumėte šablono funkcijas. Išsamius veiksmus, pavyzdžius ir aplinkybes žr. 

- [Pasirinktinio scenarijaus leidimas arba apsauga nuo jo](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda Įrašyti svetainę kaip šabloną nepalaikoma ir gali sukelti problemų svetainėse, kurios naudoja "SharePoint" publikavimo infrastruktūrą.

**Nepavyko sukurti svetainės šablono arba jis veikia netinkamai**

Šablone gali nebūti [funkcijos ir](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) jis nebus suaktyvinamas. Jei funkcijos negalima suaktyvinti dabartiniame svetainių rinkinyje, negalite naudoti svetainės šablono svetainei kurti.

- Patikrinkite, ar bet kurie sąrašai ar bibliotekos viršija sąrašo [rodinio](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ribinę 5 000 elementų ribą, nes tai gali blokuoti svetainės šablono kūrimą.

- Svetainė gali naudoti per daug išteklių, todėl svetainės šablonas viršija 50 MB limitą.


- Kyla problemų rodant duomenis iš sąrašo, kuriame naudojamas peržvalgos stulpelis. Daugiau informacijos žr. Šablonų sugeneruotas sąrašas nerodo duomenų iš tinkamo peržvalgos sąrašo [programoje "SharePoint Online".](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Išsamesnės informacijos apie įprastas problemas ir sprendimus ieškokite Svetainės [šablonų kūrimas ir naudojimas](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



