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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637785"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Valdykite fojė nustatymus ir dalyvavimo lygį

Jei norite leisti visiems, įskaitant telefono, išorinius ir anoniminius vartotojus apeiti fojė, galite naudoti "PowerShell", kad tai atlikti. Toliau pateikiame jūsų organizacijai skirtos visuotinės susitikimų strategijos modifikavimo pavyzdį.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šiuo metu cmdlet reikia naudoti "Skype" Business "PowerShell" modulis. Norėdami gauti sąrankos naudoti šį cmdlet, patikrinkite valdymo strategijos per "PowerShell".

Galite nustatyti naują strategiją, kurią turėsite taikyti vartotojams. Jei pakeisite visuotinę strategiją, ji bus automatiškai taikoma vartotojams. Bet kokiam politikos pasikeitime reikia palaukti bent 4 valandas ir iki 24 valandų, kol strategijos įsigalios.

Prieš atlikdami šiuos pakeitimus, būtinai peržiūrėkite toliau pateiktą dokumentaciją, kad tiksliai suprastumėte, ką tai leidžia.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>"Teams" susitikimų fojė strategijos valdiklių supratimas

- [Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra už organizatorius politiką, kuri kontroliuoja, ar žmonės prisijungti prie susitikimo tiesiogiai arba laukti fojė tol, kol jie priimami autentifikuotas vartotojas.

- [Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorius politika, kuri kontroliuoja, ar anoniminius žmones, įskaitant B2B ir bendrą vartotojams, gali prisijungti prie vartotojo susitikimo be autentifikuotas vartotojas iš organizacijos lankomumą.

- [Leisti telefono vartotojams apeiti fojė](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**netrukus**) yra už organizatorius politika, kuri kontroliuoja, ar žmonės, kurie rinkti telefonu prisijungti prie susitikimo tiesiogiai arba laukti fojė, nepriklausomai nuo **automatiškai priimti žmonių** nustatymas.

- [Leisti organizatoriams nepaisyti lobby parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**netrukus**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar susitikimo organizatorius gali nepaisyti fojė parametrų, kuriuos administratorius nustato **automatiškai priimti žmones** ir **leisti telefono ryšio vartotojams apeiti fojė** , kai jie Suplanuokite naują susitikimą.

**Pastaba:** Perskaitykite [tvarkyti susitikimų strategijas programoje "teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) ", kad būtų pateikta išsami "Microsoft teams" susitikimų strategijos apžvalga.
