---
title: Darbo eigos el. laiškas nesiunčiamas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766141"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbo eigos el. laiškas nesiunčiamas SharePoint sąrašui arba bibliotekai

1. El. laiškai iš darbo eigų siunčiami ne visiems vartotojams arba tik konkretiems vartotojams arba matote **klaidą El. laiško išsiųsti negalima. Įsitikinkite, kad el. laiške yra tinkamas gavėjas**.

    Patikrinkite, ar vartotojas yra to svetainių rinkinio teisių grupėje **Visi žmonės** (vartotojo informacijos sąraše).  Tiesioginio URL<tenant>pavyzdys: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0

    - Jei vartotojo nėra, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio. 
    - Jei jis yra išorinis vartotojas, įsitikinkite, kad jų kvietimas buvo priimtas.
    - Jei vartotojas yra teisių grupėje, įsitikinkite, kad el. pašto adresas yra teisingas.
    - Jei čia vartotojų el. pašto adresas nenustatytas, sukurkite to vartotojo įspėjimo pavyzdį, kuris verčia sinchronizuoti tą vartotojo abonementą iš "SharePoint" vartotojų profilių į šį svetainių rinkinį.
 
2. El. laiškas iš darbo eigų siunčiamas svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir rodoma klaida **HTTP Draudžiama <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Prieiga [uždrausta, kai siunčiate el. laišką SharePoint grupei](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Be to, patikrinkite, ar **ribotos prieigos vartotojo teisių užrakinimo režimo** svetainių rinkinio funkcija nėra aktyvi.


## <a name="related-topics"></a>Susijusios temos
Norite išbandyti "Microsoft Flow" "SharePoint Online"?
- [Kurti srautą](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- ["SharePoint" ir srautas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


