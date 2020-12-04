---
title: "\"PRT\" problemos trikčių šalinimas"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573720"
---
# <a name="troubleshoot-prt-issue"></a>"PRT" problemos trikčių šalinimas

Kad bet kuris įrenginys galėtų būti autentifikuotas, jis turi būti visiškai užregistruotas ir geras ir gali įsigyti pirminį atnaujinimo atpažinimo ženklą (PAG).

Hibridinis "Azure AD" prisijungimo procesas reikalauja, kad įrenginiai būtų taikomi kolektyviniame tinkle. Jis taip pat veikia per VPN, tačiau yra tam tikrų apribojimų. Girdėjome klientų, kuriems reikia pagalbos šalinant hibridinio "Azure AD" prisijungimo procesą pagal nuotolinio darbo sąlygas. Toliau aprašyta, kas vyksta "po gaubtu" registracijos proceso metu.

**Debesies autentifikavimo aplinka (naudojant "Azure AD" slaptažodžių maišos sinchronizavimą arba Pass-per autentifikavimą)**

Šis registracijos srautas taip pat žinomas kaip "sinchronizavimo sujungimas".

1. "Windows 10" aptinka "SCP" įrašą, kai vartotojas jungiasi prie įrenginio.
    1. Įrenginys pirmiausia bando gauti nuomotojo informaciją iš kliento "SCP" registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Jei nepavyksta, įrenginys palaiko ryšį su vietinio "Active Directory" (AD), kad gautų nuomotojo informaciją iš tarnybos jungties taško (SCP). Norėdami patikrinti, ar yra "SCP", skaitykite šį [dokumentą](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Rekomenduojame įjungti "SCP" skelbimą ir naudoti tik kliento "SCP" pradiniam patvirtinimui.

2. "Windows 10" bando palaikyti ryšį su "Azure AD" pagal sistemos kontekstą ir autentifikuoja save nuo "Azure AD". Galite patikrinti, ar įrenginys gali pasiekti "Microsoft" išteklius pagal sistemos paskyrą, naudodami bandomojo įrenginio registracijos ryšio scenarijų.

3. "Windows 10" generuoja vartotojo pasirašomą sertifikatą ir saugo jį vietiniame skelbime esančiame kompiuterio objekte. Tam reikia, kad būtų matomas domeno valdiklis.

4. Įrenginio objektas, turintis sertifikatą, bus sinchronizuotas su "Azure AD" naudojant "Azure AD Connect". Sinchronizavimo ciklas yra kas 30 minučių pagal numatytuosius parametrus, tačiau tai priklauso nuo "Azure AD Connect" konfigūracijos. Daugiau informacijos rasite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Šiame etape jums turėtų būti suteikta galimybė matyti temos įrenginį "laukianti" būsena dalyje "Azure" portalo įrenginio peilis.

6. Kitas vartotojas prisijungęs prie "Windows 10", registracija bus atlikta. 

> [!NOTE]
> Jei esate VPN ir atsijungti prisijungimo procesas nutraukia domeno ryšį, galite suaktyvinti registraciją rankiniu būdu:
 1. "Dsregcmd" (prisijungti prie kompiuterio) arba nuotoliniu būdu per PSExec prie kompiuterio. Pvz., PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Daugiau informacijos apie hibridinio sujungimo problemas ieškokite [įrenginių trikčių diagnostika](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
