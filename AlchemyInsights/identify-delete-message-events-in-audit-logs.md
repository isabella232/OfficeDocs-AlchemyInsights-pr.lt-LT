---
title: Nustatyti naikinimo pranešimų įvykius audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716504"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Panaikintų el. laiškų audito žurnalai

Nuo 2019 m. sausio , "Microsoft" įjungia pašto dėžutės audito registravimą pagal numatytuosius nustatymus. Kitu atveju, jei norite peržiūrėti konkretaus vartotojo pranešimų naikinimo įvykius, turite rankiniu būdu įgalinti tikrinimo naikinimo veiksmus. Jei pašto dėžučių audito registravimas jau įgalintas jūsų organizacijoje arba konkrečiam vartotojui, atlikite toliau nurodytus veiksmus.

1. Prisijunkite prie ["Microsoft 365" saugos & atitikties centro](https://protection.office.com/)

2. Spustelėkite **Ieškoti ir tirti** ir pasirinkite Audito **žurnalo ieška**.

3. Laukuose **Pradžios data** ir **Pabaigos data** pasirinkite dienų seką. Nurodykite vartotojo, kurį norite ištirti, vartotojo vardą (vartotoją, kuris panaikino elementus). Lauke **Veikla** pasirinkite **Panaikinti pranešimai iš aplanko Pašalinta** ir **Perkelti pranešimai į aplanką Pašalinta**.

4. Spustelėkite **Ieškoti**.

Rezultatuose pasirinkite audito įrašą. Išsamios informacijos iškeliamamejį meniu spustelėkite **Daugiau informacijos**. Papildoma informacija apie panaikintą elementą (pvz., temos eilutė ir elemento vieta, kai jis buvo panaikintas) rodoma lauke **Susijusio Elementai.** **Ypatybė ClientInfoString** bus rodoma, jei naikinimas įvyko programoje "Outlook", "Outlook" žiniatinklyje (anksčiau vadinta "Outlook Web App") ar bet kuriame kitame įrenginyje.

Daugiau informacijos [ieškokite Nustatymas, kas nustato pašto dėžutės el. pašto peradresavimą](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Pastaba:** negalite nuskaityti panaikintų elementų naudodami audito žurnalo funkciją. Norėdami nuskaityti panaikintus pranešimus internetinėje "Outlook", žiūrėkite [Panaikintų elementų atkūrimas "Outlook Web App".](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
