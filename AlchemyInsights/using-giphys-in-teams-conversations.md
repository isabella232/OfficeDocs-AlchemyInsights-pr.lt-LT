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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="2817a-102">"Giphys" naudojimas "teams" pokalbiuose</span><span class="sxs-lookup"><span data-stu-id="2817a-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="2817a-103">"Giphys" prieiga programoje "teams" yra įjungta pagal numatytuosius numatytuosius.</span><span class="sxs-lookup"><span data-stu-id="2817a-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="2817a-104">Jei esate administratorius, galite valdyti, ar "Giphys" galima naudoti vartotojams [nustatant pranešimų siuntimo strategiją](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ir užtikrinant, kad būtų **įjungta** **pokalbių** funkcija.</span><span class="sxs-lookup"><span data-stu-id="2817a-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="2817a-105">Jei "teams" pokalbiuose nedirbama kaip tikėtasi, patikrinkite:</span><span class="sxs-lookup"><span data-stu-id="2817a-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="2817a-106">[Pranešimų strategija](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) turi leisti "Giphys".</span><span class="sxs-lookup"><span data-stu-id="2817a-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="2817a-107">Norėdami patikrinti naudodami "PowerShell" "cmdlet":</span><span class="sxs-lookup"><span data-stu-id="2817a-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="2817a-108">Patikrinkite, ar galite [valdyti komandas naudodami "PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)".</span><span class="sxs-lookup"><span data-stu-id="2817a-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="2817a-109">Paleiskite "PowerShell" komandą [gauti – CsTeamsMessagingPolicy – tapatybė visuotinis](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ir patikrinkite, ar **allowgiphy** nustatytas į **TRUE (teisinga** ).</span><span class="sxs-lookup"><span data-stu-id="2817a-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="2817a-110">Jei **allowgiphy** nustatytas kaip **klaidingas** , vykdykite šią "PowerShell" komandų [rinkinį – CsTeamsMessagingPolicy – tapatybė Global – allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="2817a-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="2817a-111">Norint suteikti prieigą prie "Giphy" URL, reikia įgalinti [pasirinktines susijusias funkcijas](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .</span><span class="sxs-lookup"><span data-stu-id="2817a-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="2817a-112">Jei jūsų nuomotojui sukonfigūruota kelios "teams" pranešimų politikos strategijos, galite nustatyti, kad "PowerShell" komandos "PowerShell" komandos tapatybė turi būti priskirta prie "PowerShell" komandos [get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Pasirinkite TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="2817a-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
