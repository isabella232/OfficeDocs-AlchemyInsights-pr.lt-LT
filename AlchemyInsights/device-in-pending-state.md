---
title: Įrenginio būsena laukiama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330380"
---
# <a name="device-in-pending-state"></a>Įrenginio būsena laukiama

**Būtinosios sąlygos:**

1. Jei pirmą kartą nustatote įrenginių registracijas, įsitikinkite, kad peržiūrėjote [""Azure Active Directory"" ("Azure AD")](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) įrenginių valdymo įvadas, kuris padės jums gauti įrenginius pagal "Azure AD" valdymą.
2. Jei registruosite įrenginius į "Azure AD" tiesiogiai ir užregistruosite juos "Intune", turėsite įsitikinti, kad sukonfigūravote ["Intune"](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ir pirmiausia [turite](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) licencijavimą.
3. Įsitikinkite, kad turite teisę atlikti operacijas "Azure AD" ir vietinėje AD. Tik visuotinis „Azure AD“ administratorius gali valdyti įrenginių registravimo parametrus. Be to, jei vietiniame „Active Directory“ nustatote automatines registracijas, turėsite būti „Active Directory“ ir „AD FS“ (jei taikoma) administratorius.

Hibridinis "Azure AD" prisijungimo registracijos procesas reikalauja, kad įrenginiai būtų įmonės tinkle. Ji taip pat veikia naudojant VPN, tačiau yra tam tikrų įspėjimų. Išgirdome klientus, kuriems reikia pagalbos šalinant hibridinės "Azure AD" prisijungimo registracijos procesą nuotoliniu būdu.

**Debesies autentifikavimo aplinka (naudojant "Azure AD" slaptažodžių sinchronizavimą arba nuotolinį autentifikavimą)**

Šis registracijos srautas taip pat žinomas kaip "Sinchronizavimo prisijungimas".

Toliau pateikiamas suskirstymas, kas nutinka registracijos proceso metu:

1. Windows 10 tarnybos ryšio taško (SCP) įrašą, kai vartotojas prisijungia prie įrenginio.

    1. Įrenginys pirmiausia bando gauti nuomotojo informaciją iš kliento SCP registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Daugiau informacijos žr. [dokumentas](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Jei nepavyksta, įrenginys susisiekia su vietinę "Active Directory", kad iš SCP gautumėte nuomotojo informaciją. Norėdami patikrinti SCP, žr. šį [dokumentą](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    **Pastaba:** rekomenduojame įgalinti SCP "Active Directory" ir naudoti tik kliento SCP pradiniam patvirtinimui.

2. Windows 10 bendrauti su "Azure AD" sistemos kontekste, kad autentifikuoti save "Azure AD".

    Galite patikrinti, ar įrenginys gali pasiekti "Microsoft" išteklius sistemos paskyroje naudodamas [tikrinimo įrenginio registracijos jungiamumo scenarijų](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 sugeneruoja savarankiškai pasirašytą sertifikatą ir saugo jį po kompiuterio objektu vietinėje "Active Directory". Tam reikia regos linijos į domeno valdiklį.

4. Įrenginio objektas, kuriame yra sertifikatas, sinchronizuojamas su "Azure AD" naudojant "Azure AD" Prisijungimas. Sinchronizavimo ciklas pagal numatytuosius nustatymus yra kas 30 minučių, tačiau tai priklauso nuo "Azure AD" Prisijungimas. Daugiau informacijos žr. šiame [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Šiame etape temos įrenginį turėtumėte matyti "Azure" portalo įrenginio **ašmenų** būsenoje Laukiama.

6. Per kitą vartotojo prisijungimą prie Windows 10, registracija bus baigta.

    **Pastaba:** jei esate VPN ir atsijungti / prisijungti nutraukia domeno ryšį, galite paleisti registraciją rankiniu būdu. Norėdami tai padaryti:
    
    `dsregcmd /join`Iškiškite vietoje administratoriaus raginimą arba nuotoliniu būdu per "PSExec" savo kompiuteryje.\
    Pavyzdžiui: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Dažniausiai pasitaikančių problemų dėl "Azure Active Directory" įrenginių registracijos žr. [Įrenginių DUK](https://docs.microsoft.com/azure/active-directory/devices/faq).
