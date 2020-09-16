---
title: Neatsiųstas darbo eigos laiškas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748997"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>"SharePoint" sąrašui arba bibliotekai nesiunčiama darbo eigos el. paštas

1. El. laiškai iš darbo eigų nesiunčiami visiems vartotojams arba tik konkretiems vartotojams arba rodoma klaida, **kai el. laiško išsiųsti negalima. Įsitikinkite, kad el. laiškas turi galiojantį gavėją**.

    Patikrinkite, ar vartotojas nėra to svetainių rinkinio grupėje **Visos žmonių** teisės (vartotojų informacijos sąrašas).  Pavyzdinis tiesioginis URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Jei vartotojo nėra, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio. 
    - Jei tai išorinis vartotojas, įsitikinkite, kad jų kvietimas priimtas.
    - Jei vartotojas yra grupėje teisės, įsitikinkite, kad teisingas elektroninio pašto adresas.
    - Jei vartotojas elektroninio pašto adresas nustatytas čia, tada sukurkite įspėjimų apie tą vartotoją, kuris verčia tos vartotojo paskyros sinchronizavimą iš "SharePoint" vartotojų profilių su šiuo svetainių rinkiniu.
 
2. El. laiškai iš darbo eigų siunčiami svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir matyti klaidos **http uždraustas <span>https:</span>//URL/_vti_bin/Client.xvc.sp.utilities.Utility.sendemail**.
 

    [Jei siunčiate laišką "SharePoint" grupei, žiūrėkite prieiga uždrausta](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Taip pat patikrinkite, ar neaktyvi " **Access" vartotojo teisių blokavimo režimo** svetainių rinkinio funkcija.


## <a name="related-topics"></a>Susijusios temos
Norite išbandyti "Microsoft Flow" "SharePoint Online"?
- [Kurti srautą](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- ["SharePoint" ir srautas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


