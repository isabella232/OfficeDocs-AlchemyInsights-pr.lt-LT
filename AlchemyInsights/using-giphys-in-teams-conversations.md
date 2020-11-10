---
title: "\"Giphys\" naudojimas \"teams\" pokalbiuose"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982504"
---
# <a name="using-giphys-in-teams-conversations"></a>"Giphys" naudojimas "teams" pokalbiuose

"Giphys" prieiga programoje "teams" yra įjungta pagal numatytuosius numatytuosius. Jei esate administratorius, galite valdyti, ar "Giphys" galima naudoti vartotojams [nustatant pranešimų siuntimo strategiją](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ir užtikrinant, kad būtų **įjungta** **pokalbių** funkcija.

Jei "teams" pokalbiuose nedirbama kaip tikėtasi, patikrinkite:

[Pranešimų strategija](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) turi leisti "Giphys". Norėdami patikrinti naudodami "PowerShell" "cmdlet":

- Patikrinkite, ar galite [valdyti komandas naudodami "PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)".
- Paleiskite "PowerShell" komandą [gauti – CsTeamsMessagingPolicy – tapatybė visuotinis](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ir patikrinkite, ar **allowgiphy** nustatytas į **TRUE (teisinga** ).
- Jei **allowgiphy** nustatytas kaip **klaidingas** , vykdykite šią "PowerShell" komandų [rinkinį – CsTeamsMessagingPolicy – tapatybė Global – allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Norint suteikti prieigą prie "Giphy" URL, reikia įgalinti [pasirinktines susijusias funkcijas](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Jei jūsų nuomotojui sukonfigūruota kelios "teams" pranešimų politikos strategijos, galite nustatyti, kad "PowerShell" komandos "PowerShell" komandos tapatybė turi būti priskirta prie "PowerShell" komandos [get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pasirinkite TeamsMessagingPolicy.
