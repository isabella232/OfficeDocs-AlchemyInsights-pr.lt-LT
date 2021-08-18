---
title: Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip tai padaryti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317816"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip tai padaryti

Jei išorinis peradresavimas buvo nustatytas pašto dėžutėje, veikla audituota kaip **set-Mailbox** cmdlet dalis. Štai kaip rasti veiklą audito žurnale:

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras , <https://compliance.microsoft.com> eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> , eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://security.microsoft.com/auditlogsearch> .

   **Pastaba:** jei matote pranešimą, kad reikia įjungti auditą, eikite į priekį ir įjunkite jį dabar. Jei ši funkcija neįjungta, ieškos rezultatai negalės gauti duomenų iš ankstesnių datų.

2. Puslapyje **Tikrinimas** patikrinkite, ar pažymėtas **skirtukas** Ieška, tada sukonfigūruokite šiuos parametrus:
   - Laukuose Pradžia ir Pabaiga pasirinkite **datos /** **laiko diapazoną.**
   - Patikrinkite, **ar lauke** Veikla yra Rodyti visų **veiklų rezultatus.**

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje.

4. Rezultatuose spustelėkite stulpelį Veikla, **kad** surikiuotume rezultatus, ir ieškokite **Set-Mailbox įrašų.**

5. Pasirinkite veiklą rezultatuose, kad atidarytumėte išsamios informacijos iškelia į lauką. Turite peržiūrėti kiekvieno audito įrašo informaciją, kad nustatytumėte, ar veikla susijusi su el. pašto peradresavimu:
   - **ObjectId**: modifikuotos pašto dėžutės pseudonimo reikšmė.
   - **Parametrai**: _ForwardingSmtpAddress_ nurodo tikslinį el. pašto adresą.
   - **UserId**: vartotojas, kuris sukonfigūravo el. pašto peradresavimą lauke **ObjectId.**

Daugiau informacijos žr. [Pašto dėžutės el. pašto peradresavimo nustatymas](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
