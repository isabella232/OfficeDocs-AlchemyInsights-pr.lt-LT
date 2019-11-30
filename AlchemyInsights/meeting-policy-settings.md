---
title: Susitikimų strategijos parametrai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627582"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Tvarkykite susitikimų strategijas programoje "Microsoft teams"

Susitikimų strategijos naudojamos valdyti funkcijoms, kurios pasiekiamos jūsų organizacijos vartotojų suplanuotų susitikimų dalyviams. Kai kurios susitikimų strategijos funkcijos "teams" administravimo centre gali būti neįgyvendintos (tai yra pažymėta "netrukus" dokumentacijoje). Tokiu atveju arba, jei gaunate klaidos pranešimą "negalime atnaujinti strategijos dabar, bet bandykite ją dar kartą" Microsoft teams "administravimo centras, rekomenduojame naudoti" PowerShell "komandų susitikimo strategijų kūrimas arba modifikavimas. 

Daugiau informacijos apie susitikimų strategijas rasite šiuose šaltiniuose:

- Norėdami sužinoti, kaip kurti strategijas, atlikti keitimus ir priskirti vartotojus politikai [, žr.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Norėdami, kad strategijos pakeitimai naudojant "PowerShell" cmdlet, ieškokite [komandos "PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Jums reikia naudoti ["Skype" Business PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) komandų susitikimo strategijos. 
    - Peržiūrėkite [*-csteamsmeetingpolicy cmdlet dokumentaciją](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) daugiau informacijos.

**Pastaba:** Tai gali užtrukti iki 24 valandų, kad politikos pakeitimai įsigaliotų vartotojams. Gali nepavykti iš karto keisti naujai sukurtų strategijų; Palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą politiką. Jei vis tiek kyla problemų, bandykite "PowerShell".  