---
title: Susitikimo strategijos parametrai
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925173"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Susitikimo strategijų valdymas "Microsoft Teams

**Pastaba: gali užtrukti iki 24 valandų, kad strategijos pakeitimai įsigalios vartotojams.** Jums gali nepavykti iš karto atlikti naujai sukurtų strategijų pakeitimų; palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą strategiją.

Susitikimų strategijos naudojamos valdyti funkcijas, kurios susitikimo dalyviams prieinamos susitikimams, kuriuos suplanuoja jūsų organizacijos vartotojai. Kai kurios susitikimų strategijų funkcijos dar gali būti Teams administravimo centre (dokumentuose jos žymimos "netrukus"). Šiuo atveju arba jei "Microsoft Teams" administravimo centre gaunate klaidą, pvz., "Šiuo metu negalime atnaujinti strategijos, bet bandykite ją dar kartą vėliau", rekomenduojame naudoti "PowerShell", kad sukurtumėte arba pakeistumėte "Teams" susitikimų strategijas. 

Daugiau informacijos apie susitikimų strategijas žr. šie ištekliai:

- Norėdami sužinoti apie strategijų kūrimas, keitimų keitimų ir vartotojų priskyrimą strategijai, žr. [Susitikimų strategijų valdymas Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Norėdami keisti strategiją naudodami "PowerShell" "cmdlet", [žr. Teams "PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Jums reikia naudoti ["PowerShell"Skype" verslui "PowerShell" modulį,](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) kad Teams susitikimo strategijas. 
    - Daugiau informacijos [žr. *-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentacijoje.

