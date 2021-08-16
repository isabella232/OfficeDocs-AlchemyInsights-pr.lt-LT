---
title: Darbo eigos el. laiškas nesiunčiamas
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072528"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbo eigos el. laiškas nesiunčiamas SharePoint sąrašui arba bibliotekai

1. El. laiškai iš darbo eigų nesiunčiami visiems vartotojams arba tik konkretiems vartotojams arba matote klaidą El. laiško išsiųsti **negalima. Įsitikinkite, kad el. laiške yra galiojantis gavėjas.**

    Patikrinkite, ar vartotojas yra to **svetainių rinkinio** teisių grupėje Visi žmonės (vartotojų informacijos sąrašas).  Tiesioginio URL pavyzdys: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Jei vartotojo nėra, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio. 
    - Jei tai išorinis vartotojas, įsitikinkite, kad jo kvietimas buvo priimtas.
    - Jei vartotojas yra teisių grupėje, įsitikinkite, kad teisingas el. pašto adresas.
    - Jei vartotojų el. pašto adresas čia nėra nustatytas, sukurkite to vartotojo įspėjimo pavyzdį, kuris verčia to vartotojo paskyros sinchronizavimą iš "SharePoint profilių į šį svetainių rinkinį.
 
2. El. laiškai iš darbo eigų siunčiami svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir žr. klaidą HTTP Draudžiama **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Žr. [Prieiga uždrausta, kai siunčiate el. laišką į SharePoint grupę.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Taip pat patikrinkite, ar **ribotos prieigos vartotojo teisių blokavimo režimo** svetainių rinkinio funkcija nėra aktyvi.


## <a name="related-topics"></a>Susijusios temos
Norite išbandyti "Microsoft Flow" "SharePoint Online"?
- [Kurti Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ir Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


