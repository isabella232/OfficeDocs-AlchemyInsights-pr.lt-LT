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
# <a name="control-lobby-settings-and-level-of-participation"></a>Valdykite fojė nustatymus ir dalyvavimo lygį

Šie parametrai kontroliuoja, kurie susitikimų dalyviai laukia fojė prieš priimant į susitikimą, ir jų dalyvavimo susitikime lygį. Naudodami "PowerShell" galite atnaujinti susitikimų strategijos parametrus, kurie dar neįdiegti (pažymėti "netrukus") "teams" administravimo centre.  Žiūrėkite žemiau pavyzdys PowerShell cmdlet, kuri leidžia visiems vartotojams apeiti fojė.  

- [Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra už organizatorius politiką, kuri kontroliuoja, ar žmonės prisijungti prie susitikimo tiesiogiai arba laukti fojė tol, kol jie priimami autentifikuotas vartotojas.

- [Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorius politika, kuri kontroliuoja, ar anoniminius žmones, įskaitant B2B ir bendrą vartotojams, gali prisijungti prie vartotojo susitikimo be autentifikuotas vartotojas iš organizacijos lankomumą.

- [Leisti telefono vartotojams apeiti fojė](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**netrukus**) yra už organizatorius politika, kuri kontroliuoja, ar žmonės, kurie rinkti telefonu prisijungti prie susitikimo tiesiogiai arba laukti fojė, nepriklausomai nuo **automatiškai priimti žmonių** nustatymas.

- [Leisti organizatoriams nepaisyti lobby parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**netrukus**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar susitikimo organizatorius gali nepaisyti fojė parametrų, kuriuos administratorius nustato **automatiškai priimti žmones** ir **leisti telefono ryšio vartotojams apeiti fojė** , kai jie Suplanuokite naują susitikimą.

**Pastaba:** Perskaitykite [tvarkyti susitikimų strategijas programoje "teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) ", kad būtų pateikta išsami "Microsoft teams" susitikimų strategijos apžvalga. 


**"PowerShell" pavyzdys**

Jei norite leisti visiems, įskaitant išorinius arba anoniminius vartotojus, apeiti fojė, taip pat galite naudoti "PowerShell" šiai užduočiai atlikti.  Toliau pateikiame jūsų organizacijai skirtos visuotinės susitikimų strategijos modifikavimo pavyzdį.   

(Prieš atlikdami šiuos pakeitimus, būtinai Peržiūrėkite anksčiau pateiktus dokumentus, kad tiksliai suprastumėte, ką tai leidžia daryti.)

Set-CsTeamsMeetingPolicy-tapatybės Global-AutoAdmittedUsers "visi"-AllowPSTNUsersToBypassLobby $True

Daugiau informacijos ieškokite [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
