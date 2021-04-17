---
title: Aplinkkelio laukiamajame
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820042"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="12ea7-102">Valdykite fojė parametrus ir dalyvavimo "Teams" lygį</span><span class="sxs-lookup"><span data-stu-id="12ea7-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="12ea7-103">Jei norite leisti visiems, įskaitant skambinimo, išorinius ir anoniminius vartotojus, **apeiti** laukiamąjį , šiai užduočiai atlikti naudokite "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="12ea7-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="12ea7-104">Štai jūsų organizacijos visuotinio susitikimo strategijos modifikavimo pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="12ea7-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="12ea7-105">Šiai "cmdlet" šiuo metu reikia naudoti "Skype" verslui "PowerShell" modulį.</span><span class="sxs-lookup"><span data-stu-id="12ea7-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="12ea7-106">Norėdami nustatyti naudoti šią "cmdlet", peržiūrėkite Strategijų [valdymas naudojant "PowerShell".](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="12ea7-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="12ea7-107">Nustatę strategiją, turite ją taikyti vartotojams; arba, jei modifikavote visuotinę strategiją, ji bus automatiškai taikoma vartotojams.</span><span class="sxs-lookup"><span data-stu-id="12ea7-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="12ea7-108">Jei norite pakeisti strategiją, turite palaukti bent **4 valandas iki 24 valandų,** kol strategijos įsigalios.</span><span class="sxs-lookup"><span data-stu-id="12ea7-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="12ea7-109">Prieš pradėdami šiuos pakeitimus, būtinai peržiūrėkite toliau pateiktą dokumentaciją, kad tiksliai suprastumėte, ką tai leidžia.</span><span class="sxs-lookup"><span data-stu-id="12ea7-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="12ea7-110">"Teams" susitikimo laukiame strategijos valdiklių supratimas</span><span class="sxs-lookup"><span data-stu-id="12ea7-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="12ea7-111">Šie parametrai valdo, kurie susitikimo dalyviai laukiame, kol jiems bus leista dalyvauti susitikime, ir dalyvavimo susitikime lygį.</span><span class="sxs-lookup"><span data-stu-id="12ea7-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="12ea7-112">"PowerShell" galite naudoti norėdami atnaujinti dar neįgyvendintas susitikimo strategijos parametrus (pavadintus "netrukus") "Teams" administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="12ea7-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="12ea7-113">Žr. toliau pateiktą pavyzdį "PowerShell" cmdlet, kuri leidžia visiems vartotojams apeiti laukiamąjį.</span><span class="sxs-lookup"><span data-stu-id="12ea7-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="12ea7-114">[Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra organizatoriaus strategija, kuri kontroliuoja, ar žmonės prisijungia prie susitikimo tiesiogiai, ar laukia, kol juos priima autentifikuotas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="12ea7-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="12ea7-115">[Leisti anoniminiams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) žmonėms pradėti susitikimą yra organizatoriaus strategija, kuri kontroliuoja, ar anoniminiai žmonės, įskaitant B2B ir išorinius vartotojus, gali prisijungti prie vartotojo susitikimo be autentifikuoto vartotojo iš organizacijos.</span><span class="sxs-lookup"><span data-stu-id="12ea7-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="12ea7-116">Leisti konferencinio skambinimo vartotojams apeiti laukiamąjį **(** jau greitai ) yra organizatoriaus strategija, kuri kontroliuoja, ar žmonės, kurie skambina telefonu, prisijungia prie susitikimo tiesiogiai arba laukia laukiamajame, neatsižvelgiant į parametrą Automatiškai **priimti** [žmones.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)</span><span class="sxs-lookup"><span data-stu-id="12ea7-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="12ea7-117">[Leisti organizatoriams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) nepaisyti laukiamųjų parametrų **(** jau greitai ) yra organizatoriaus strategija, kuri kontroliuoja,  ar susitikimo organizatorius gali nepaisyti laukiamajame parametrų, kuriuos administratorius nustatė dalyje Automatiškai priimti **žmones** ir Leisti skambinimo vartotojams apeiti laukiamąjį, kai jie suplanuoja naują susitikimą.</span><span class="sxs-lookup"><span data-stu-id="12ea7-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="12ea7-118">**Pastaba:** Skaitykite ["Teams" susitikimų strategijų valdymas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) ir išsami "Microsoft Teams" susitikimų strategijų apžvalga.</span><span class="sxs-lookup"><span data-stu-id="12ea7-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
