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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104316"
---
# <a name="using-giphys-in-teams-conversations"></a>"Giphys" naudojimas Teams pokalbiuose

Pagal numatytuosius nustatymus "Giphys" Teams pokalbio prieiga yra įjungta. Jei esate administratorius, galite kontroliuoti, ar "Giphys" yra pasiekiami vartotojams, nustatydami pranešimų strategiją ir užtikrindami, **kad "Giphys" naudojimas pokalbiuose yra** **On**. [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)

Jei GIF neveikia taip, kaip tikėtasi, Teams pokalbiuose, patikrinkite:

Pranešimų [strategija turi leisti](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) "Giphys". Norėdami patikrinti naudodami "PowerShell" "cmdlet":

- Patikrinkite, ar galite [valdyti Teams "PowerShell".](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Vykdykite komandą ["PowerShell" Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ir patikrinkite, **ar AllowGiphy** nustatyta kaip **TRUE**.
- Jei **AllowGiphy** nustatyta kaip **FALSE**, vykdykite šią "PowerShell" komandą [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Norint suteikti prieigą prie](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) "Giphy" URL, būtina įgalinti pasirinktines prijungtas funkcijas.

> [!NOTE]
> Jei nuomotojui sukonfigūruota Teams pranešimų strategija, galite nustatyti paveiktam vartotojui priskirtos strategijos tapatybę naudodami [komandą "PowerShell" Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pasirinkite TeamsMessagingPolicy.
