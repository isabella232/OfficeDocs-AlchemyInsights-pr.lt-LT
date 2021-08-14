---
title: Pranešimo įvykių naikinimas audito žurnaluose
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868426"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Panaikintų el. laiškų audito žurnalai

Nuo 2019 m. sausio "Microsoft" įjungia pašto dėžutės audito registravimą pagal numatytuosius parametrus. Kitu atveju, norėdami peržiūrėti konkretaus vartotojo pranešimų naikinimo įvykius, turite rankiniu būdu įgalinti tikrinimo naikinimo veiksmus. Jei pašto dėžutės audito registravimas jau įgalintas jūsų organizacijoje arba konkrečiam vartotojui, atlikite toliau nurodytus veiksmus.

1. Prisijunkite prie ["Microsoft 365 atitikties centro](https://protection.office.com/)

2. Spustelėkite **Ieška ir tyrimas ir** pasirinkite Audito **žurnalo ieška**.

3. Pasirinkite datos diapazoną **laukuose Pradžios data** ir **Pabaigos** data. Nurodykite vartotojo, kurį norite ištirti, vartotojo vardą (vartotoją, kuris panaikins elementus). Lauke **Veikla pasirinkite** Panaikinti laiškai **iš** aplanko Panaikinti elementai ir Perkelti laiškai į aplanką **Panaikinti elementai**.

4. Spustelėkite **Ieškoti**.

Rezultatuose pasirinkite audito įrašą. Išsamios informacijos iškeliame meniu spustelėkite **Daugiau informacijos**. Lauke **AffectedItems** rodoma papildoma informacija apie panaikintą elementą (pvz., temos eilutė ir elemento vieta, kai jis buvo panaikintas). Ypatybė **ClientInfoString** rodys, ar naikinimas įvyko Outlook, internetinė "Outlook" (anksčiau vadinosi Outlook Web App) ar bet kuriuo kitu įrenginiu.

Daugiau informacijos žr. [Pašto dėžutės el. pašto peradresavimo nustatymas](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Pastaba:** negalite gauti panaikintų elementų naudodami audito žurnalo funkciją. Norėdami gauti panaikintus internetinė "Outlook", [žr. Panaikintų elementų atkūrimas Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
