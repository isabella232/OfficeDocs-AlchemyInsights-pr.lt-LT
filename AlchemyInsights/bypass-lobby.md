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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059604"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Valdykite fojė parametrus ir dalyvavimo Teams

Jei norite leisti visiems, įskaitant skambinimo, išorinius ir anoniminius vartotojus, **apeiti** laukiamąjį , šiai užduočiai atlikti naudokite "PowerShell". Štai jūsų organizacijos visuotinio susitikimo strategijos modifikavimo pavyzdys.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Šiai "cmdlet" šiuo metu reikia naudoti ""Skype" verslui"PowerShell" modulį. Norėdami nustatyti naudoti šią "cmdlet", peržiūrėkite Strategijų [valdymas naudojant "PowerShell".](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Nustatę strategiją, turite ją taikyti vartotojams; arba, jei modifikavote visuotinę strategiją, ji bus automatiškai taikoma vartotojams. Jei norite pakeisti strategiją, turite palaukti bent **4 valandas iki 24 valandų,** kol strategijos įsigalios. 

Prieš pradėdami šiuos pakeitimus, būtinai peržiūrėkite toliau pateiktą dokumentaciją, kad tiksliai suprastumėte, ką tai leidžia.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Susitikimų Teams lobistų strategijos valdiklių supratimas

Šie parametrai valdo, kurie susitikimo dalyviai laukiame, kol jiems bus leista dalyvauti susitikime, ir dalyvavimo susitikime lygį. "PowerShell" galite naudoti norėdami atnaujinti dar neįgyvendintas susitikimo strategijos parametrus (pažymėtus "netrukus") Teams administravimo centre. Žr. toliau pateiktą pavyzdį "PowerShell" cmdlet, kuri leidžia visiems vartotojams apeiti laukiamąjį.

- [Automatiškai priimti žmones](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) yra organizatoriaus strategija, kuri kontroliuoja, ar žmonės prisijungia prie susitikimo tiesiogiai, ar laukia, kol juos priima autentifikuotas vartotojas.

- [Leisti anoniminiams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) žmonėms pradėti susitikimą yra organizatoriaus strategija, kuri kontroliuoja, ar anoniminiai žmonės, įskaitant B2B ir išorinius vartotojus, gali prisijungti prie vartotojo susitikimo be autentifikuoto vartotojo iš organizacijos.

- Leisti konferencinio skambinimo vartotojams apeiti laukiamąjį **(** jau greitai ) yra organizatoriaus strategija, kuri kontroliuoja, ar žmonės, kurie skambina telefonu, prisijungia prie susitikimo tiesiogiai arba laukia laukiamajame, neatsižvelgiant į parametrą Automatiškai **priimti** [žmones.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)

- [Leisti organizatoriams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) nepaisyti laukiamųjų parametrų **(** jau greitai ) yra organizatoriaus strategija, kuri kontroliuoja,  ar susitikimo organizatorius gali nepaisyti laukiamajame parametrų, kuriuos administratorius nustatė dalyje Automatiškai priimti **žmones** ir Leisti skambinimo vartotojams apeiti laukiamąjį, kai jie suplanuoja naują susitikimą.

**Pastaba:** Skaitykite [Susitikimų strategijų valdymas Teams,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) kad būtų galima peržiūrėti Microsoft Teams susitikimų strategijas.
