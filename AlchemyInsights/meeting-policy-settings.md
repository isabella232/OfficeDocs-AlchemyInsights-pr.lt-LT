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
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376736"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Tvarkykite susitikimų strategijas programoje "Microsoft teams"

Susitikimų strategijos naudojamos valdyti funkcijoms, kurios pasiekiamos jūsų organizacijos vartotojų suplanuotų susitikimų dalyviams. Kai kurios susitikimų strategijos funkcijos "teams" administravimo centre gali būti neįgyvendintos (tai yra pažymėta "netrukus" dokumentacijoje). Tokiu atveju arba, jei gaunate klaidos pranešimą "negalime atnaujinti strategijos dabar, bet bandykite ją dar kartą" Microsoft teams "administravimo centras, rekomenduojame naudoti" PowerShell "komandų susitikimo strategijų kūrimas arba modifikavimas. 

Daugiau informacijos apie susitikimų strategijas rasite šiuose šaltiniuose:

- Norėdami sužinoti, kaip kurti strategijas, atlikti keitimus ir priskirti vartotojus politikai [, žr.](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)

- Norėdami, kad strategijos pakeitimai naudojant "PowerShell" cmdlet, ieškokite [komandos "PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Jums reikia naudoti ["Skype" Business PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) komandų susitikimo strategijos. 
    - Peržiūrėkite [*-csteamsmeetingpolicy cmdlet dokumentaciją](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) daugiau informacijos.

**Pastaba:** Tai gali užtrukti iki 24 valandų, kad politikos pakeitimai įsigaliotų vartotojams. Gali nepavykti iš karto keisti naujai sukurtų strategijų; Palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą politiką. Jei vis tiek kyla problemų, bandykite "PowerShell".  