---
title: Viršytas dienos el. pašto limitas. Darbo eiga sustabdoma.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731571"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Viršytas dienos el. pašto limitas. Darbo eiga sustabdoma.

Ši klaida gali būti gauta šiais atvejais:

- Naudojate "SharePoint Online" darbo eigą, kuri naudoja "SharePoint 2010" arba "SharePoint 2013" darbo eigos platformos tipą.
- Darbo eiga sukonfigūruota siųsti pasirinktiniam el. laiškui daugiau nei 200 vartotojams vienu metu, daugiau nei 10 000 gavėjams per dieną arba daugiau nei 30 pranešimų per minutę.
- Paleidus darbo eigą, el. laiškas neatsiųstas, o jūs pastebėsite tokį veikimą:
    - Jei naudojate darbo eigą naudodami "SharePoint" 2013 platformos tipą, pereikite į **darbo eigos būsenos** puslapį. Darbo eigos būsenos puslapyje **Vidinė būsena** nustatyta kaip **paleista**, o informacijos debesėlyje rodoma **negalima išsiųsti gavėjui**.

Norėdami išspręsti šią problemą, sukonfigūruokite darbo eigą, kad siųstumėte el. laiškus, neviršijant " [Exchange Online" siuntėjo limitų](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Pvz., naudokite darbo eigą pristabdyti, siųskite el. laišką į "Microsoft" 365 grupę, platinimo grupę arba pašto įgalintos saugos grupę arba išsiųskite laišką mažiau nei "200" gavėjams vienu metu.


Daugiau informacijos ieškokite šiame [straipsnyje](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Susijusios temos
- [Kurti srautą](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- ["SharePoint" ir srautas](https://flow.microsoft.com/blog/sharepoint-and-flow/) 