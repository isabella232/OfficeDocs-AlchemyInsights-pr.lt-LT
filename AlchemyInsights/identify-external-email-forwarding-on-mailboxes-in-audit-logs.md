---
title: Išorinių laiškų peradresavimo pašto dėžutėse nustatymas audito žurnaluose
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696305"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Atpažinimas, kai išoriniai pašto peradresavimas yra sukonfigūruotas pašto dėžutėse

Kai "Microsoft 365" vartotojo konfigūruoja išorinį el. pašto peradresavimą pašto dėžutėje, veikla tikrinama kaip **Set-Mailbox** cmdlet dalis. Galite peržiūrėti veiklą naudodami audito žurnalų iešką saugos & atitikties centre.

1. Prisijungimas prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/).

2. Eikite į puslapį **ieškos**  >  **audito žurnalų ieška** .

3. Laukuose **pradžios data** ir **pabaigos data** pasirinkite datų intervalą. Jums nereikia įvesti vartotojo vardo. Patikrinkite, ar laukas **veikla** nustatytas **Rodyti visų veiklų rezultatus**.

4. Spustelėkite **ieška**.

Rezultatuose spustelėkite **filtruoti rezultatus** ir įveskite **Set-Mailbox** lauke veiklos filtras. Rezultatuose pasirinkite audito įrašą. **Išsamios informacijos** išskridimas spustelėkite **daugiau informacijos**. Turite pažiūrėti kiekvieno audito įrašo išsamią informaciją, kad nustatytumėte, ar veikla susijusi su elektroninio pašto peradresavimu.

- **ObjectId**: pakeistos pašto dėžutės pseudonimo reikšmė.

- **Parametrai**: " _forwardingsmt paddress_ " nurodo tikslinį elektroninio pašto adresą.

- **UserID**: vartotojas, sukonfigūravęs pašto peradresavimo funkciją lauke **ObjectId** .

Daugiau informacijos ieškokite kaip [nustatyti, kas nustato pašto dėžutės pašto peradresavimą](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
