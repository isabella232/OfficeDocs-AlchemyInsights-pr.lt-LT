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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376741"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="cf299-102">Valdykite fojė nustatymus ir dalyvavimo lygį</span><span class="sxs-lookup"><span data-stu-id="cf299-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="cf299-103">Šie parametrai kontroliuoja, kurie susitikimų dalyviai laukia fojė prieš priimant į susitikimą, ir jų dalyvavimo susitikime lygį.</span><span class="sxs-lookup"><span data-stu-id="cf299-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="cf299-104">Naudodami "PowerShell" galite atnaujinti susitikimų strategijos parametrus, kurie dar neįdiegti (pažymėti "netrukus") "teams" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="cf299-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="cf299-105">Žiūrėkite žemiau pavyzdys PowerShell cmdlet, kuri leidžia visiems vartotojams apeiti fojė.</span><span class="sxs-lookup"><span data-stu-id="cf299-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="cf299-106">[Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra už organizatorius politiką, kuri kontroliuoja, ar žmonės prisijungti prie susitikimo tiesiogiai arba laukti fojė tol, kol jie priimami autentifikuotas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="cf299-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="cf299-107">[Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorius politika, kuri kontroliuoja, ar anoniminius žmones, įskaitant B2B ir bendrą vartotojams, gali prisijungti prie vartotojo susitikimo be autentifikuotas vartotojas iš organizacijos lankomumą.</span><span class="sxs-lookup"><span data-stu-id="cf299-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="cf299-108">[Leisti telefono vartotojams apeiti fojė](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**netrukus**) yra už organizatorius politika, kuri kontroliuoja, ar žmonės, kurie rinkti telefonu prisijungti prie susitikimo tiesiogiai arba laukti fojė, nepriklausomai nuo **automatiškai priimti žmonių** nustatymas.</span><span class="sxs-lookup"><span data-stu-id="cf299-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="cf299-109">[Leisti organizatoriams nepaisyti lobby parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**netrukus**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar susitikimo organizatorius gali nepaisyti fojė parametrų, kuriuos administratorius nustato **automatiškai priimti žmones** ir **leisti telefono ryšio vartotojams apeiti fojė** , kai jie Suplanuokite naują susitikimą.</span><span class="sxs-lookup"><span data-stu-id="cf299-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="cf299-110">**Pastaba:** Perskaitykite [tvarkyti susitikimų strategijas programoje "teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) ", kad būtų pateikta išsami "Microsoft teams" susitikimų strategijos apžvalga.</span><span class="sxs-lookup"><span data-stu-id="cf299-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="cf299-111">**"PowerShell" pavyzdys**</span><span class="sxs-lookup"><span data-stu-id="cf299-111">**PowerShell example**</span></span>

<span data-ttu-id="cf299-112">Jei norite leisti visiems, įskaitant išorinius arba anoniminius vartotojus, apeiti fojė, taip pat galite naudoti "PowerShell" šiai užduočiai atlikti.</span><span class="sxs-lookup"><span data-stu-id="cf299-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="cf299-113">Toliau pateikiame jūsų organizacijai skirtos visuotinės susitikimų strategijos modifikavimo pavyzdį.</span><span class="sxs-lookup"><span data-stu-id="cf299-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="cf299-114">(Prieš atlikdami šiuos pakeitimus, būtinai Peržiūrėkite anksčiau pateiktus dokumentus, kad tiksliai suprastumėte, ką tai leidžia daryti.)</span><span class="sxs-lookup"><span data-stu-id="cf299-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="cf299-115">Set-CsTeamsMeetingPolicy-tapatybės Global-AutoAdmittedUsers "visi"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="cf299-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="cf299-116">Daugiau informacijos ieškokite [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="cf299-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
