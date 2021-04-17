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
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836359"
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
