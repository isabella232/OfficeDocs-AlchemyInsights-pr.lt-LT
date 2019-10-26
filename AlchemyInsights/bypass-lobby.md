---
title: Aplinkkelis fojė
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/25/2019
ms.locfileid: "37654264"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="2c7fe-102">Valdykite fojė nustatymus ir dalyvavimo lygį</span><span class="sxs-lookup"><span data-stu-id="2c7fe-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="2c7fe-103">Jei norite leisti visiems, įskaitant telefono, išorinius ir anoniminius vartotojus apeiti fojė, galite naudoti "PowerShell", kad tai atlikti.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="2c7fe-104">Toliau pateikiame jūsų organizacijai skirtos visuotinės susitikimų strategijos modifikavimo pavyzdį.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="2c7fe-105">Šiuo metu cmdlet reikia naudoti "Skype" Business "PowerShell" modulis.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="2c7fe-106">Norėdami gauti sąrankos naudoti šį cmdlet, patikrinti [valdymo strategijos per "PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)".</span><span class="sxs-lookup"><span data-stu-id="2c7fe-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="2c7fe-107">Galite nustatyti naują strategiją, kurią turėsite taikyti vartotojams.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="2c7fe-108">Jei pakeisite visuotinę strategiją, ji bus automatiškai taikoma vartotojams.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="2c7fe-109">Bet kokiam politikos pasikeitime reikia palaukti bent 4 valandas ir iki 24 valandų, kol strategijos įsigalios.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="2c7fe-110">Prieš atlikdami šiuos pakeitimus, būtinai peržiūrėkite toliau pateiktą dokumentaciją, kad tiksliai suprastumėte, ką tai leidžia.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="2c7fe-111">"Teams" susitikimų fojė strategijos valdiklių supratimas</span><span class="sxs-lookup"><span data-stu-id="2c7fe-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="2c7fe-112">[Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra už organizatorius politiką, kuri kontroliuoja, ar žmonės prisijungti prie susitikimo tiesiogiai arba laukti fojė tol, kol jie priimami autentifikuotas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="2c7fe-113">[Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorius politika, kuri kontroliuoja, ar anoniminius žmones, įskaitant B2B ir bendrą vartotojams, gali prisijungti prie vartotojo susitikimo be autentifikuotas vartotojas iš organizacijos lankomumą.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="2c7fe-114">[Leisti telefono vartotojams apeiti fojė](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**netrukus**) yra už organizatorius politika, kuri kontroliuoja, ar žmonės, kurie rinkti telefonu prisijungti prie susitikimo tiesiogiai arba laukti fojė, nepriklausomai nuo **automatiškai priimti žmonių** nustatymas.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="2c7fe-115">[Leisti organizatoriams nepaisyti lobby parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**netrukus**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar susitikimo organizatorius gali nepaisyti fojė parametrų, kuriuos administratorius nustato **automatiškai priimti žmones** ir **leisti telefono ryšio vartotojams apeiti fojė** , kai jie Suplanuokite naują susitikimą.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="2c7fe-116">**Pastaba:** Perskaitykite [tvarkyti susitikimų strategijas programoje "teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) ", kad būtų pateikta išsami "Microsoft teams" susitikimų strategijos apžvalga.</span><span class="sxs-lookup"><span data-stu-id="2c7fe-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
