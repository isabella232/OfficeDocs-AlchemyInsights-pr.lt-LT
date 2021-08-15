---
title: Ištaisyti klaidą Programa neaptikta
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
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026122"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Ištaisyti klaidą „Programa neaptikta“

Programos diegimo klaida „Programa nebuvo aptikta po sėkmingo įdiegimo“, apie kurią praneša „Intune“, gali įvykti visose pagrindinėse OS platformose („Windows“, „iOS“ ir „Android“).

Dažniausi scenarijai, kurie sugeneruoja šią klaidą, apima:

- Programa buvo atnaujinta ne iš „Intune“ (trečiosios šalies programų parduotuvės) po pradinio diegimo. Pvz., kai kurios programos, kaip „Google Chrome“, gali atlikti automatinius naujinimus.
- Vartotojas pašalino programą po pradinio diegimo.

Norėdami išspręsti šią problemą, pirmiausia atlikite susijusių įrenginių apžvalgą, kad nustatytumėte scenarijų, kuriuo įvyksta klaida.

- Jei programa buvo atnaujinta ne iš „Intune“, programos diegimas gali būti nustatytas nepaisyti programos versijos. Norėdami tai padaryti, dalyje **Programų konfigūravimas > Programos informacija** nustatykite **Nepaisyti programos** versijos į **Taip**.
- Orientuojantis į klientą gali būti tikslinga diegti taikomąją programą kaip „būtiną“ ir užtikrinti, kad būtų įdiegta naujausia versija.
- Be to, „iOS“ platformoje galima naudoti **automatinio naujinimo** funkcines galimybes, susietas su „Apple Volume“ pirkimo programa, kurią galima konfigūruoti automatiškai atnaujinti į naujas programų versijas, kai jos bus pasiekiamos.

Jei reikia daugiau informacijos apie programų diegimo trikčių šalinimą, žr. [Programų diegimo problemų šalinimas](https://docs.microsoft.com/intune/troubleshoot-app-install).
