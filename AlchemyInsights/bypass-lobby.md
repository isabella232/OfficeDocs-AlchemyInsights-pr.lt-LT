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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Valdykite fojė nustatymus ir dalyvavimo programoje "teams" lygį

Jei norite leisti visiems, įskaitant telefono, išorinius ir anoniminius vartotojus, **apeiti fojė**, Norėdami atlikti šią užduotį, naudokite "PowerShell". Toliau pateikiame jūsų organizacijai skirtos visuotinės susitikimų strategijos modifikavimo pavyzdį.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šiuo metu cmdlet reikia naudoti "Skype" Business "PowerShell" modulis. Norėdami nustatyti naudoti šį cmdlet, patikrinkite [valdymo strategijos per "PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)".

Nustatę strategiją, turite ją taikyti vartotojams; arba, jei modifikavote pasaulinę politiką, ji bus automatiškai taikoma vartotojams. Jei norite, kad politikos pakeitimas įsigaliotų, turite palaukti mažiausiai **4 valandas iki 24 valandų** . 

Prieš atlikdami šiuos pakeitimus, būtinai peržiūrėkite toliau pateiktą dokumentaciją, kad tiksliai suprastumėte, ką tai leidžia.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>"Teams" susitikimų fojė strategijos valdiklių supratimas

Šie parametrai kontroliuoja, kurie susitikimų dalyviai laukia fojė prieš priimant į susitikimą, ir jų dalyvavimo susitikime lygį. Naudodami "PowerShell" galite naujinti susitikimų strategijos parametrus, kurie dar neįdiegti (pažymėti "netrukus") komandos administravimo centre. Žiūrėkite žemiau pavyzdys PowerShell cmdlet, kuri leidžia visiems vartotojams apeiti fojė.

- [Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra už organizatorius politiką, kuri kontroliuoja, ar žmonės prisijungti prie susitikimo tiesiogiai arba laukti fojė tol, kol jie priimami autentifikuotas vartotojas.

- [Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorius politika, kuri kontroliuoja, ar anoniminius žmones, įskaitant B2B ir bendrą vartotojams, gali prisijungti prie vartotojo susitikimo be autentifikuotas vartotojas iš organizacijos lankomumą.

- [Leisti telefono vartotojams apeiti fojė](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**netrukus**) yra už organizatorius politika, kuri kontroliuoja, ar žmonės, kurie rinkti telefonu prisijungti prie susitikimo tiesiogiai arba laukti fojė, nepriklausomai nuo **automatiškai priimti žmonių** nustatymas.

- [Leisti organizatoriams nepaisyti lobby parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**netrukus**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar susitikimo organizatorius gali nepaisyti fojė parametrų, kuriuos administratorius nustato **automatiškai priimti žmones** ir **leisti telefono vartotojams apeiti fojė** , kai jie Suplanuokite naują susitikimą.

**Pastaba:** Perskaitykite [tvarkyti susitikimų strategijas programoje "teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) ", kad būtų pateikta išsami "Microsoft teams" susitikimų strategijos apžvalga.
