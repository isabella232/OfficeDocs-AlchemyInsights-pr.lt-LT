---
title: Išorinio el. pašto peradresavimo pašto dėžutėse tikrinimas audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331167"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Nustatyti, kada išorinis el. pašto peradresavimas sukonfigūruotas pašto dėžutėse

Kai Microsoft 365 sukonfigūruoja išorinį el. pašto peradresavimą pašto dėžutėje, veikla audituojamas kaip **"cmdlet" set-Mailbox** dalis. Galite matyti veiklą naudodami audito žurnalo iešką. Štai kaip tai padaryti.

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras , <https://compliance.microsoft.com> eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> , eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://sip.security.microsoft.com/auditlogsearch> .

2. Puslapyje **Tikrinimas** patikrinkite, ar pažymėtas **skirtukas** Ieška, tada sukonfigūruokite šiuos parametrus:
   - Laukuose Pradžia ir Pabaiga pasirinkite **datos /** **laiko diapazoną.**
   - Patikrinkite, **ar lauke** Veikla yra Rodyti visų **veiklų rezultatus.**

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje.

4. Rezultatuose spustelėkite **Filtruoti rezultatus ir** veiklos filtro lauke įveskite **Set-Mailbox.**

5. Pasirinkite audito įrašą rezultatuose. **Iškeliame** meniu Išsami informacija spustelėkite **Daugiau informacijos**. Turite peržiūrėti kiekvieno audito įrašo informaciją, kad nustatytumėte, ar veikla susijusi su el. pašto peradresavimu.

   - **ObjectId**: modifikuotos pašto dėžutės pseudonimo reikšmė.
   - **Parametrai**: _ForwardingSmtpAddress_ nurodo tikslinį el. pašto adresą.
   - **UserId**: vartotojas, kuris sukonfigūravo el. pašto peradresavimą lauke **ObjectId.**

Daugiau informacijos žr. [Pašto dėžutės el. pašto peradresavimo nustatymas](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
