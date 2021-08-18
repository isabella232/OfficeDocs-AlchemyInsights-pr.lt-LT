---
title: "\"Giphys\" naudojimas Teams pokalbiuose"
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323528"
---
# <a name="using-giphys-in-teams-conversations"></a>"Giphys" naudojimas Teams pokalbiuose

Pagal numatytuosius nustatymus "Giphys" Teams pokalbio prieiga yra įjungta. Jei esate administratorius, galite kontroliuoti, ar "Giphys" yra pasiekiami vartotojams, nustatydami pranešimų strategiją ir užtikrindami, **kad "Giphys" naudojimas pokalbiuose yra** **On**. [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)

Jei GIF neveikia taip, kaip tikėtasi, Teams pokalbiuose, patikrinkite:

Pranešimų [strategija turi leisti](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) "Giphys". Norėdami patikrinti naudodami "PowerShell" "cmdlet":

- Patikrinkite, ar galite [valdyti Teams "PowerShell".](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Vykdykite komandą ["PowerShell" Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ir patikrinkite, **ar AllowGiphy** nustatyta kaip **TRUE**.
- Jei **AllowGiphy** nustatyta kaip **FALSE**, vykdykite šią "PowerShell" komandą [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Norint suteikti prieigą prie](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) "Giphy" URL, būtina įgalinti pasirinktines prijungtas funkcijas.

**Pastaba:** jei turite kelias Teams pranešimų strategijas, sukonfigūruotas nuomotojui, galite nustatyti paveiktam vartotojui priskirtos strategijos tapatybę naudodami [komandą "PowerShell" Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pasirinkite TeamsMessagingPolicy.
