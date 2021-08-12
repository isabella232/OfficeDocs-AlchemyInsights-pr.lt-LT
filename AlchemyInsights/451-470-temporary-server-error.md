---
title: 451 4.7.0 Laikinojo serverio klaida. Bandykite dar kartą vėliau. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812584"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Laikinojo serverio klaida. Bandykite dar kartą vėliau. PRX4

Galite susidurti su problema siųsdami el. laiškus per "Smarthost" "smtp.office365.com" naudodami SMTP kliento pateikimo metodą ir gaunate klaidą: "451 4.7.0 Temporary server error" (451 4.7.0 laikinojo serverio klaida). Bandykite dar kartą vėliau. PRX4 dažniausiai yra laikinas." 

Įsitikinkite, kad nenaudojate bendrinamos pašto dėžutės SMTP kliento pateikimui, nes SMTP kliento pateikimo metodui reikia licencijuotos pašto dėžutės, kad būtų galima siųsti laiškus. Tačiau, jei nenaudojate bendrinamos pašto dėžutės ir problema išlieka, patikrinkite šiuos veiksmus:

1. Įgalinkite kliento SMTP pateikimą licencijuotos pašto dėžutės, kuri naudojama vykdant šią "PowerShell" komandą:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    ARBA

    1. Eikite į "Microsoft 365" administravimo centras > **aktyvūs** vartotojai ir pasirinkite vartotoją.
    1. Eikite į skirtuką Paštas, > **El.** pašto > pasirinkite Tvarkyti **el. pašto programas.** 
    1. Įsitikinkite, kad **pažymėtas parametras** Autentifikuotas SMTP (įgalintas).
    1. Pasirinkite **Įrašyti keitimus**.
    
    Norėdami įgalinti SMTP autentifikavimą visoje organizacijoje, vykdykite šią komandą:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Pastaba:** saugos sumetimais rekomenduojama įgalinti SMTP autentifikavimą tik naudojamai pašto dėžutei. Vartotojo lygio parametras perrašo organizacijos lygio parametrą.

2. Išjunkite "Azure" saugos numatytąsias reikšmes, norėdami įjungti **saugos numatytąsias reikšmes į** **Ne:**

    1. Prisijunkite prie "Azure" portalo kaip saugos administratorius, sąlyginės prieigos administratorius arba visuotinis administratorius.
    1. Raskite "Azure Active Directory" >**  Ypatybės** ir pasirinkite **Valdyti saugos numatytąsias reikšmes**.
    1. Nustatykite **jungiklį Įjungti saugos numatytąsias reikšmes** kaip **Ne**.
    1. Pasirinkite **Įrašyti**.

3. Išjunkite kelių dalių autentifikavimą (MFA) licencijuotose naudojamose pašto dėžutėse.

    1. Eikite į "Microsoft 365" administravimo centras ir kairiajame naršymo meniu pasirinkite Vartotojai  >  **aktyvūs vartotojai**.
    1. Puslapyje **Aktyvūs vartotojai** pasirinkite Kelių **dalių autentifikavimas**.
    1. Pasirinkite vartotoją ir išjunkite **kelių dalių autentifikavimą**.

