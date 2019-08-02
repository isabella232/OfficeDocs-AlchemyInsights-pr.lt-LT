---
title: Darbo eigos paštu nesiunčiamas
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059611"
---
# <a name="workflow-email-is-not-being-sent"></a>Darbo eigos paštu nesiunčiamas

1. El. paštas darbo eigos siunčiami visiems vartotojams arba tik tam tikriems vartotojams, arba matote klaidos **el. laiško negalima išsiųsti. Įsitikinkite, kad el. laiškas turi galiojantį gavėją**.

Patikrinti, ar vartotojas yra **Visų žmonių** teises grupės (vartotojo informacijos sąraše) šio svetainių rinkinio.  Paragauti tiesiogiai URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Jei vartotojas nėra, įsitikinkite, kad vartotojas yra prisijungę prie puslapio. 
- Jeigu išorinis vartotojas, įsitikinkite, kad jų kvietimą buvo priimtas.
- Jei vartotojas teisės grupė, įsitikinkite, ar teisingas el. pašto adresas.
- Jei vartotojai el. pašto adresas nėra nustatytas čia, tada sukurti iš mėginio signalą, kad vartotojas, kuris verčia šio vartotojo abonemento sinchronizavimo SharePoint vartotojo profiliai prie šio svetainių rinkinio.
 
2. El. paštas darbo eigos siunčiami svetainių rinkinio administratoriai, bet ne kitiems vartotojams ir pamatyti klaidos **HTTP draudžiama į <spam> <spam> ** <spam> <spam>.
 

Žiūrėkite [Prieiga uždrausta kai išsiųstą el. laišką dalyvauja](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Be to, įsitikinkite, kad **riboto naudojimo vartotojas leidimo lockdown režimas** svetainių rinkinio funkcija neaktyvi.

## <a name="related-topics"></a>Susijusios temos
- [Sukurti srauto](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ir srauto](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


