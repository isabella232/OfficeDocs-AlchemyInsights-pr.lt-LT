---
title: Viršytas dienos el. pašto limitas. Darbo eiga sustabdyta.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914659"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Viršytas dienos el. pašto limitas. Darbo eiga sustabdyta.

Ši klaida gali būti gauta šiais atvejais:

- Turite darbo eigą "SharePoint Online", kuri naudoja "SharePoint 2010" arba "SharePoint 2013" darbo eigos platformos tipą.
- Darbo eiga sukonfigūruota siųsti pasirinktinį el. laišką daugiau nei 200 vartotojų vienu metu, daugiau nei 10 000 gavėjų per dieną arba daugiau nei 30 pranešimų per minutę.
- Paleidus darbo eigą, el. laiškas nesiunčiamas ir pastebite tokį veikimą:
    - Norėdami naudoti darbo eigą naudodami SharePoint 2013 m. platformos tipą, eikite į puslapį **Darbo eigos būsena.** Puslapyje Darbo eigos būsena nustatyta **Vidinė būsena** kaip Paleista , **o** informacijos debesėlis **rodo Nepavyko išsiųsti gavėjui**.

Norėdami išspręsti šią problemą, sukonfigūruokite savo darbo eigą, kad siųsdami [el. laiškus neviršydami Exchange Online siuntėjų apribojimų.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Pvz., darbo eigoje naudokite pauzę, siųskite el. laišką "Microsoft 365" grupei, siuntimo grupei arba pašto saugos grupei arba išsiųskite pranešimą mažiau nei 200 gavėjų vienu metu.


Daugiau informacijos žr. šiame [straipsnyje](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Susijusios temos
- [Kurti Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ir Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 