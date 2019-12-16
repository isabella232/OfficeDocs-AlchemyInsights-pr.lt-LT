---
title: Nesiunčiamas darbo eigos el. laiškas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049381"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Darbo eigos el. laiškas nesiunčiamas SharePoint sąrašui arba bibliotekai

1. El. laiškai iš darbo eigų nesiunčiami visiems vartotojams arba tik konkretiems vartotojams, arba matote klaidą **, kurios negalima siųsti el. laišku. Įsitikinkite, kad el. laiške yra galiojantis gavėjas**.

    Patikrinkite, ar vartotojas yra **visų asmenų** teisių grupės (vartotojo informacijos sąraše), kad svetainių rinkinio.  Imties tiesioginė URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0

    - Jei vartotojas neegzistuoja, įsitikinkite, kad vartotojas yra prisijungęs prie puslapio. 
    - Jei tai išorinis naudotojas, įsitikinkite, kad jo kvietimas buvo priimtas.
    - Jei teisių grupėje yra vartotojas, įsitikinkite, kad el. pašto adresas teisingas.
    - Jei vartotojų el. pašto adresas čia nenustatytas, tada sukurkite įspėjimą apie pavyzdį tam vartotojui, kuris priverčia to vartotojo abonemento sinchronizavimą iš "SharePoint" vartotojo profilių į šį svetainių rinkinį.
 
2. El. laiškai iš darbo eigų siunčiami svetainių rinkinio administratoriams, bet ne kitiems vartotojams ir rodoma klaida **http uždrausta <span>https:</span>//URL/_vti_bin/Client.xvc.sp.utilities.Utility.sendemail**.
 

    Peržiūrėkite [prieiga uždrausta siunčiant el. laišką į SharePoint grupę](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Be to, patikrinkite, ar nėra aktyvus **ribotos prieigos vartotojo teisių blokavimo režimu** svetainių rinkinio funkcija.


## <a name="related-topics"></a>Susijusios temos
Norite išbandyti "Microsoft Flow" "SharePoint Online"?
- [Sukurti srautą](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- ["SharePoint" ir srautas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


