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
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825451"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>"Microsoft Teams" susitikimų strategijų valdymas

**Pastaba: gali užtrukti iki 24 valandų, kad strategijos pakeitimai įsigalios vartotojams.** Jums gali nepavykti iš karto atlikti naujai sukurtų strategijų pakeitimų; palaukite 4 valandas ir dar kartą bandykite modifikuoti naujai sukurtą strategiją.

Susitikimų strategijos naudojamos valdyti funkcijas, kurios susitikimo dalyviams prieinamos susitikimams, kuriuos suplanuoja jūsų organizacijos vartotojai. Kai kurios susitikimų strategijų funkcijos dar gali būti neį įgyvendinamos "Teams" administravimo centre (dokumentuose jos žymimos "netrukus"). Šiuo atveju arba jei gaunate klaidos pranešimą, pvz., "Šiuo metu negalime atnaujinti strategijos, bet bandykite ją dar kartą vėliau" "Microsoft Teams" administravimo centre, rekomenduojame naudoti "PowerShell" "Teams" susitikimų strategijai kurti arba modifikuoti. 

Daugiau informacijos apie susitikimų strategijas žr. šie ištekliai:

- Norėdami sužinoti apie strategijų kūrimas, pakeitimų keitimų ir vartotojų priskyrimą strategijai, žr. [Susitikimų strategijų valdymas "Teams".](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Norėdami keisti strategiją naudodami "PowerShell" "cmdlet", žr. ["Teams PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Turite naudoti ["Skype" verslui "PowerShell" modulį, skirtą "Teams"](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) susitikimo strategijai. 
    - Daugiau informacijos [žr. *-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentacijoje.

