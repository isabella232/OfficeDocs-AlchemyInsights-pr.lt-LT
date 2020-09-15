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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Lobby parametrų valdymas ir dalyvavimo grupėse lygis

Jei norite leisti visiems, įskaitant skambinimą, išorinius ir anoniminius vartotojus, **apeiti laukiamąjį**, naudokite "PowerShell", kad galėtumėte atlikti šią užduotį. Pateikiame savo organizacijos visuotinio susitikimo strategijos modifikavimo pavyzdį.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šiuo metu šiai "cmdlet" reikia naudoti "Skype" verslui "PowerShell" modulį. Norėdami nustatyti naudoti šią "cmdlet", peržiūrėkite strategijas naudodami " [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)".

Kai nustatysite strategiją, turite ją pritaikyti vartotojams; arba, jei modifikavote pasaulinę strategiją, ji bus automatiškai taikoma vartotojams. Norėdami pakeisti strategiją, turite palaukti bent **4 valandas iki 24 valandų** , kad įsigaliotų strategijos. 

Būtinai peržiūrėkite toliau pateiktus dokumentus prieš atlikdami šiuos pokyčius ir Supraskite, ką tai leidžia.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>"Teams" susitikimo vestibiulio strategijos valdiklių supratimas

Šie parametrai kontroliuoja, kurie susitikimo dalyviai laukia laukiamajame, kol jie bus įtraukti į susitikimą, ir dalyvavimo, į kurį jie leidžiami susitikime, lygį. Galite naudoti "PowerShell", jei norite atnaujinti susitikimo strategijos parametrus, kurie dar nebuvo įdiegti (pažymėti "jau greitai") komandų administravimo centre. Toliau pateiktas pavyzdys "PowerShell" cmdlet, leidžianti visiems vartotojams apeiti laukiamąjį.

- [Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) pagal organizatoriaus strategiją, kuri kontroliuoja, ar žmonės prisijungia prie susitikimo tiesiogiai, ar laukti laukiamajame, kol juos priims autentifikuotas vartotojas.

- [Leisti anoniminiams žmonėms pradėti susitikimą](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) yra už organizatorių strategija, kuri kontroliuoja, ar anoniminiai žmonės, įskaitant B2B ir susietieji vartotojai, gali prisijungti prie vartotojo susitikimo be autentifikuoto vartotojo iš organizacijos lankomumo.

- [Leisti skambinimo vartotojams apeiti laukiamąjį](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**jau greitai**) yra kiekvienos organizatoriaus strategija, kuri kontroliuoja, ar žmonės, skambinantys telefonu, prisijungia prie susitikimo tiesiogiai arba laukti laukiamajame, nepriklausomai nuo to, ar **automatiškai priimti žmonės** .

- [Leisti organizatoriams nepaisyti laukiamųjų parametrų](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**jau greitai**) yra kiekvienos organizatoriaus strategija, valdanti, ar susitikimo organizatorius gali nepaisyti "lobby" parametrų, kuriuos administratorius nustatė **automatiškai priimti žmones** ir **leisti skambinimo vartotojams apeiti laukiamąjį** , kai suplanuojamas naujas susitikimas.

**Pastaba:** Skaitykite " [teams" susitikimų strategijų valdymas](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , kad peržiūrėtumėte visą "Microsoft teams" susitikimo strategijų apžvalgą.
