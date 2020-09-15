---
title: Aplinkkelio vestibiulis
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684958"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="5bb14-102">Lobby parametrų valdymas ir dalyvavimo grupėse lygis</span><span class="sxs-lookup"><span data-stu-id="5bb14-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="5bb14-103">Jei norite leisti visiems, įskaitant skambinimą, išorinius ir anoniminius vartotojus, **apeiti laukiamąjį**, naudokite "PowerShell", kad galėtumėte atlikti šią užduotį.</span><span class="sxs-lookup"><span data-stu-id="5bb14-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="5bb14-104">Pateikiame savo organizacijos visuotinio susitikimo strategijos modifikavimo pavyzdį.</span><span class="sxs-lookup"><span data-stu-id="5bb14-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="5bb14-105">Šiuo metu šiai "cmdlet" reikia naudoti "Skype" verslui "PowerShell" modulį.</span><span class="sxs-lookup"><span data-stu-id="5bb14-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="5bb14-106">Norėdami nustatyti naudoti šią "cmdlet", peržiūrėkite strategijas naudodami " [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)".</span><span class="sxs-lookup"><span data-stu-id="5bb14-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="5bb14-107">Kai nustatysite strategiją, turite ją pritaikyti vartotojams; arba, jei modifikavote pasaulinę strategiją, ji bus automatiškai taikoma vartotojams.</span><span class="sxs-lookup"><span data-stu-id="5bb14-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="5bb14-108">Norėdami pakeisti strategiją, turite palaukti bent **4 valandas iki 24 valandų** , kad įsigaliotų strategijos.</span><span class="sxs-lookup"><span data-stu-id="5bb14-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="5bb14-109">Būtinai peržiūrėkite toliau pateiktus dokumentus prieš atlikdami šiuos pokyčius ir Supraskite, ką tai leidžia.</span><span class="sxs-lookup"><span data-stu-id="5bb14-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="5bb14-110">"Teams" susitikimo vestibiulio strategijos valdiklių supratimas</span><span class="sxs-lookup"><span data-stu-id="5bb14-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="5bb14-111">Šie parametrai kontroliuoja, kurie susitikimo dalyviai laukia laukiamajame, kol jie bus įtraukti į susitikimą, ir dalyvavimo, į kurį jie leidžiami susitikime, lygį.</span><span class="sxs-lookup"><span data-stu-id="5bb14-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="5bb14-112">Galite naudoti "PowerShell", jei norite atnaujinti susitikimo strategijos parametrus, kurie dar nebuvo įdiegti (pažymėti "jau greitai") komandų administravimo centre.</span><span class="sxs-lookup"><span data-stu-id="5bb14-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="5bb14-113">Toliau pateiktas pavyzdys "PowerShell" cmdlet, leidžianti visiems vartotojams apeiti laukiamąjį.</span><span class="sxs-lookup"><span data-stu-id="5bb14-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="5bb14-114">[Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) pagal organizatoriaus strategiją, kuri kontroliuoja, ar žmonės prisijungia prie susitikimo tiesiogiai, ar laukti laukiamajame, kol juos priims autentifikuotas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="5bb14-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5bb14-115">[Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorių strategija, kuri kontroliuoja, ar anoniminiai žmonės, įskaitant B2B ir susietieji vartotojai, gali prisijungti prie vartotojo susitikimo be autentifikuoto vartotojo iš organizacijos lankomumo.</span><span class="sxs-lookup"><span data-stu-id="5bb14-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5bb14-116">[Leisti skambinimo vartotojams apeiti laukiamąjį](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jau greitai**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar žmonės, skambinantys telefonu, prisijungia prie susitikimo tiesiogiai arba laukti laukiamajame, nepriklausomai nuo to, ar **automatiškai priimti žmonės** .</span><span class="sxs-lookup"><span data-stu-id="5bb14-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5bb14-117">[Leisti organizatoriams nepaisyti laukiamųjų parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**jau greitai**) yra kiekvienos organizatoriaus strategija, valdanti, ar susitikimo organizatorius gali nepaisyti "lobby" parametrų, kuriuos administratorius nustatė **automatiškai priimti žmones** ir **leisti skambinimo vartotojams apeiti laukiamąjį** , kai suplanuojamas naujas susitikimas.</span><span class="sxs-lookup"><span data-stu-id="5bb14-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5bb14-118">**Pastaba:** Skaitykite " [teams" susitikimų strategijų valdymas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , kad peržiūrėtumėte visą "Microsoft teams" susitikimo strategijų apžvalgą.</span><span class="sxs-lookup"><span data-stu-id="5bb14-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
