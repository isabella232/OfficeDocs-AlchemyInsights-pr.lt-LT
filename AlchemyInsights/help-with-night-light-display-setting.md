---
title: Pagalba nustatant nakties šviesos rodymo parametrą
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404666"
---
# <a name="help-with-the-night-light-display-setting"></a>Pagalba nustatant nakties šviesos rodymo parametrą

Norėdami sužinoti daugiau apie nakties rodymo parametrus, žr. Nakties laiko nustatymas [sistemoje "Windows 10".](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Jei nakties šviesos parinktys yra pilkos dalyje Parametrai, patikrinkite ekrano tvarkyklę: 

1. Spustelėkite užduočių juostos ieškos lauką ir įveskite **Įrenginių tvarkytuvė**, tada ieškos rezultatuose **pasirinkite** Įrenginių tvarkytuvė.
1. Išplėskite **Rodymo adapteriai**. 

Deja, nakties šviesos funkcija negalima, jei jūsų įrenginys naudoja "DisplayLink" tvarkyklę arba bazinę rodymo tvarkyklę.

Nakties šviesos funkcija naudoja naujausias grafikos technologijas, todėl gali tekti atnaujinti ekrano tvarkyklę:  

- Patikrinkite, ar yra naujinimų, nueikite **į Pradžia**  >  **Parametrai**  >  **Naujinimas &**  >  **"Windows Update"**  >  **patikrinkite, ar yra naujinimų.**  

ARBA

- Apsilankykite aparatūros gamintojo palaikymo svetainėje, kad rankiniu būdu atsisiųstumėte ir įdiegtumėte naujausias rodymo tvarkykles.

## <a name="reset-night-light-in-the-registry"></a>Iš naujo nustatykite nakties šviesą registre

Jei atnaujinus ekrano tvarkyklę nepavyko, gali tekti iš naujo nustatyti nakties šviesą registre.  

**Dėmesio:** Šis trikčių šalinimo veiksmas rekomenduojamas tik pažengusiems vartotojams. Jei netinkamai modifikuojate registrą, gali kilti rimtų problemų. Jei reikia papildomos apsaugos, prieš modifikuodami registrą sukurkite atsarginę jo kopiją, kad galėsite jį atkurti, jei kyla problemų.

1. Ieškos lauke įveskite **regedit**, tada ieškos rezultatuose **pasirinkite** Registro rengyklė.

1. Eikite į šį registro raktą: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Eksportuokite ir panaikinkite šį dalinį raktą:$$windows.data.bluelightreduction.bluelightreductionstate

1. Eksportuokite ir panaikinkite šį dalinį raktą:$$windows.data.bluelightreduction.settings

1. Iš naujo paleiskite "Windows" ir patikrinkite, ar yra nakties šviesos parinkčių.


