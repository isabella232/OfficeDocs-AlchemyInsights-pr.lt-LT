---
title: PRT trikčių šalinimas
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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972724"
---
# <a name="troubleshoot-prt-issue"></a>PRT trikčių šalinimas

Kad bet kuris įrenginys baigtų autentifikuoti, jis turi būti visiškai užregistruotas ir geros būsenos ir turėti pirminį atnaujinimo atpažinimo ženklą (PRT).

Hibridinis "Azure AD" prisijungimo registracijos procesas reikalauja, kad įrenginiai būtų įmonės tinkle. Ji taip pat veikia naudojant VPN, tačiau yra tam tikrų įspėjimų. Išgirdome klientus, kuriems reikia pagalbos dėl hibridinio "Azure AD" prisijungimo prie registracijos proceso trikčių šalinimo nuotolinio darbo sąlygomis. Toliau pateikiame, kas vyksta "po gaubtu" registracijos proceso metu.

**Debesies autentifikavimo aplinka (naudojant "Azure AD" slaptažodžių sinchronizavimą arba nuotolinį autentifikavimą)**

Šis registracijos srautas taip pat žinomas kaip "Sinchronizavimo prisijungimas".

1. Windows 10 SCP įrašą vartotojui prisijungiant prie įrenginio.
    1. Įrenginys pirmiausia bando gauti nuomotojo informaciją iš kliento SCP registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Daugiau informacijos žr. šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Jei nepavyksta, įrenginys susisiekia su vietinę "Active Directory" (AD) ir gauna nuomotojo informaciją iš tarnybos ryšio taško (SCP). Norėdami patikrinti SCP, žr. šį [dokumentą](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Rekomenduojame įgalinti SCP AD ir naudoti tik kliento SCP pradiniam patvirtinimui.

2. Windows 10 " bando bendrauti su "Azure AD" sistemos kontekste, kad autentifikuoti save "Azure AD". Galite patikrinti, ar įrenginys gali pasiekti "Microsoft" išteklius sistemos paskyroje naudodamas tikrinimo įrenginio registracijos jungiamumo scenarijų.

3. Windows 10 sugeneruoja automatiškai pasirašytą sertifikatą ir saugo jį po kompiuterio objektu vietiniame AD. Tam reikia regos linijos į domeno valdiklį.

4. Įrenginio objektas, kuriame yra sertifikatas, sinchronizuojamas su "Azure AD" naudojant "Azure AD" Prisijungimas. Sinchronizavimo ciklas pagal numatytuosius nustatymus yra kas 30 minučių, tačiau tai priklauso nuo "Azure AD" Prisijungimas. Daugiau informacijos žr. šiame [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Šiame etape temos įrenginį turėtumėte matyti "Azure" portalo įrenginio ašmenų būsenoje Laukiama.

6. Kitame vartotojo prisijungime prie Windows 10, registracija bus baigta. 

> [!NOTE]
> Jei naudojate VPN ir prisijungimo prie logotipo procesas nutraukia domeno ryšį, galite paleisti registraciją rankiniu būdu:
 1. Išduokite dsregcmd /join lokaliai administratoriaus raginimą arba nuotoliniu būdu per "PSExec" į kompiuterį. Pvz., PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Daugiau informacijos apie hibridinio sujungimo problemas žr. [Įrenginių trikčių šalinimas](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
