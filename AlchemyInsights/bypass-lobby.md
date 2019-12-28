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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889090"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="facb8-102">Valdykite fojė nustatymus ir dalyvavimo programoje "teams" lygį</span><span class="sxs-lookup"><span data-stu-id="facb8-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="facb8-103">Jei norite leisti visiems, įskaitant telefono, išorinius ir anoniminius vartotojus, **apeiti fojė**, Norėdami atlikti šią užduotį, naudokite "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="facb8-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="facb8-104">Toliau pateikiame jūsų organizacijai skirtos visuotinės susitikimų strategijos modifikavimo pavyzdį.</span><span class="sxs-lookup"><span data-stu-id="facb8-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="facb8-105">Šiuo metu cmdlet reikia naudoti "Skype" Business "PowerShell" modulis.</span><span class="sxs-lookup"><span data-stu-id="facb8-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="facb8-106">Norėdami nustatyti naudoti šį cmdlet, patikrinkite [valdymo strategijos per "PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)".</span><span class="sxs-lookup"><span data-stu-id="facb8-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="facb8-107">Nustatę strategiją, turite ją taikyti vartotojams; arba, jei modifikavote pasaulinę politiką, ji bus automatiškai taikoma vartotojams.</span><span class="sxs-lookup"><span data-stu-id="facb8-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="facb8-108">Jei norite, kad politikos pakeitimas įsigaliotų, turite palaukti mažiausiai **4 valandas iki 24 valandų** .</span><span class="sxs-lookup"><span data-stu-id="facb8-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="facb8-109">Prieš atlikdami šiuos pakeitimus, būtinai peržiūrėkite toliau pateiktą dokumentaciją, kad tiksliai suprastumėte, ką tai leidžia.</span><span class="sxs-lookup"><span data-stu-id="facb8-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="facb8-110">"Teams" susitikimų fojė strategijos valdiklių supratimas</span><span class="sxs-lookup"><span data-stu-id="facb8-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="facb8-111">Šie parametrai kontroliuoja, kurie susitikimų dalyviai laukia fojė prieš priimant į susitikimą, ir jų dalyvavimo susitikime lygį.</span><span class="sxs-lookup"><span data-stu-id="facb8-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="facb8-112">Naudodami "PowerShell" galite naujinti susitikimų strategijos parametrus, kurie dar neįdiegti (pažymėti "netrukus") komandos administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="facb8-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="facb8-113">Žiūrėkite žemiau pavyzdys PowerShell cmdlet, kuri leidžia visiems vartotojams apeiti fojė.</span><span class="sxs-lookup"><span data-stu-id="facb8-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="facb8-114">[Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra už organizatorius politiką, kuri kontroliuoja, ar žmonės prisijungti prie susitikimo tiesiogiai arba laukti fojė tol, kol jie priimami autentifikuotas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="facb8-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="facb8-115">[Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorius politika, kuri kontroliuoja, ar anoniminius žmones, įskaitant B2B ir bendrą vartotojams, gali prisijungti prie vartotojo susitikimo be autentifikuotas vartotojas iš organizacijos lankomumą.</span><span class="sxs-lookup"><span data-stu-id="facb8-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="facb8-116">[Leisti telefono vartotojams apeiti fojė](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**netrukus**) yra už organizatorius politika, kuri kontroliuoja, ar žmonės, kurie rinkti telefonu prisijungti prie susitikimo tiesiogiai arba laukti fojė, nepriklausomai nuo **automatiškai priimti žmonių** nustatymas.</span><span class="sxs-lookup"><span data-stu-id="facb8-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="facb8-117">[Leisti organizatoriams nepaisyti lobby parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**netrukus**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar susitikimo organizatorius gali nepaisyti fojė parametrų, kuriuos administratorius nustato **automatiškai priimti žmones** ir **leisti telefono vartotojams apeiti fojė** , kai jie Suplanuokite naują susitikimą.</span><span class="sxs-lookup"><span data-stu-id="facb8-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="facb8-118">**Pastaba:** Perskaitykite [tvarkyti susitikimų strategijas programoje "teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) ", kad būtų pateikta išsami "Microsoft teams" susitikimų strategijos apžvalga.</span><span class="sxs-lookup"><span data-stu-id="facb8-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
