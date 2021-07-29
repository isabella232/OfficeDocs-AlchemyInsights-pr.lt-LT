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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630257"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Nustatyti, kada išorinis el. pašto peradresavimas sukonfigūruotas pašto dėžutėse

Kai Microsoft 365 sukonfigūruoja išorinį el. pašto peradresavimą pašto dėžutėje, veikla audituojamas kaip **"cmdlet" set-Mailbox** dalis. Veiklą galite matyti naudodami audito žurnalo iešką saugos & centre.

1. Prisijunkite prie ["Microsoft 365 centro.](https://protection.office.com/)

2. Eikite į **ieškos**  >  **audito žurnalo ieškos** puslapį.

3. Pasirinkite datos diapazoną **laukuose Pradžios data** ir **Pabaigos** data. Nereikia nurodyti vartotojo vardo. Patikrinkite, **ar lauke** Veikla nustatyta Rodyti visų **veiklų rezultatus.**

4. Spustelėkite **Ieškoti**.

Rezultatuose spustelėkite **Filtruoti rezultatus ir** veiklos filtro lauke įveskite **Set-Mailbox.** Pasirinkite audito įrašą rezultatuose. **Iškeliame** meniu Išsami informacija spustelėkite **Daugiau informacijos**. Turite peržiūrėti kiekvieno audito įrašo informaciją, kad nustatytumėte, ar veikla susijusi su el. pašto peradresavimu.

- **ObjectId**: modifikuotos pašto dėžutės pseudonimo reikšmė.

- **Parametrai**: _ForwardingSmtpAddress_ nurodo tikslinį el. pašto adresą.

- **UserId**: vartotojas, kuris sukonfigūravo el. pašto peradresavimą lauke **ObjectId.**

Daugiau informacijos žr. [Pašto dėžutės el. pašto peradresavimo nustatymas](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
