---
title: Rezervavimo atšaukimas
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819700"
---
# <a name="cancelling-reservation"></a>Rezervavimo atšaukimas

- **Savitarnos paslauga:** Rezervuotąjį egzempliorių galite atšaukti arba pakeisti patys naudodami ["Azure" portalą.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Pasirinkite rezervavimą ir spustelėkite grąžinti arba keisti. Atkreipkite dėmesį, kad turite turėti savininko prieigą rezervavimo užsakyme, kad galėtumėte pakeisti arba grąžinti pinigus. Prieiga prie tik rezervavimo neleis jums grąžinti pinigų arba pakeisti. Paprašykite rezervavimo užsakymo savininko suteikti jums savininko prieigą prie rezervavimo užsakymo
- **"Exchange" strategija:** Galite pakeisti kito to paties tipo rezervavimo rezervavimą – už **rezervavimo mainus nėra** jokių baudos. Bendras įsipareigojimas su nauja rezervacija turėtų būti didesnis už valiutos keitimo rezervavimo grąžinimo sumą ir būsimus mėnesinius mokėjimus (jei taikoma)
- **Grąžinimo strategija:** Pinigų grąžinimo ir atšauktų būsimų mokėjimų suma negali viršyti 50 000 JAV dolerių 12 mėnesių einamojo laikotarpio lange. Šiuo metu **neįeisime jokių baudos už pinigų** grąžinimą, bet galėtume ją apmokestinti už būsimas grąžinamąsias išmokas  
    **Išimtys:** "Us Government Enterprise Agreement" klientams negalimas apsikeitimas savitarnos paslaugomis ir atšaukimo galimybės
- **API / PS / CLI** palaikymas negalimas atšaukimo ir pinigų grąžinimo savitarnos mainams ir [pinigų grąžinimui už "Azure Reservations"](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- "Us Government Enterprise Agreement" klientams negalimas apsikeitimas savitarnos paslaugomis ir atšaukimo galimybė. Palaikomi kiti JAV vyriausybės prenumeratos tipai, įskaitant "Pay-As-You-Go" ir CSP

Sužinokite daugiau : [Kaip apdorojamos grąžinimo ir keitimo operacijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Sužinokite daugiau: ["Exchange" ir pinigų grąžinimo strategijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Kiti klausimai: [aplankykite rezervuotųjų egzempliorių dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange an existing reserved instance (Self-service)**

Galite pakeisti kito to paties tipo rezervavimo rezervavimą. Be to, jei jums jo nebereikia, galite grąžinti iki 50 000 JAV dolerių per metus. "Us Government Enterprise Agreement" klientams negalimas apsikeitimas savitarnos paslaugomis ir atšaukimo galimybė. Palaikomi kiti JAV vyriausybės prenumeratos tipai, įskaitant "Pay-As-You-Go" ir CSP. Turite turėti savininko prieigą rezervavimo užsakyme, kad galėtumėte pakeisti esamą rezervavimą arba jį grąžinti.

Toliau nurodyti veiksmai padės atlikti operaciją

1. Prisijunkite prie ["Azure" portalo](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pasirinkite užsakymus, kuriuos norite grąžinti, ir spustelėkite **"Exchange"**
2. Pasirinkite VM produktą, kurį norite įsigyti, ir įveskite kiekį. Įsitikinkite, kad nauja pirkimo suma yra didesnė už grąžinamą sumą [Nustatykite tinkamą dydį prieš pirkdami](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Operacijos peržiūra ir pabaigti

**Rezervuotųjų egzempliorių grąžinimas**

Norėdami grąžinti rezervaciją, eikite į **Išsami rezervavimo informacija** ir spustelėkite **Grąžinti**

**Pro-rated refund:**

**Grąžinimo ir keitimo reikalavimo pavyzdžiai ir minimalūs reikalavimai**  
Išankstinio rezervavimo pavyzdys:

- Sausio 1 d. įsigyjate vienų metų trukmės RI už 120 EUR
- Balandžio 7 d. norite grąžinti pinigus arba pakeisti šį rezervavimą
- Kadangi rezervavimas buvo gyvas 97 dienas, gausite (1-97/365) * 120 EUR atgal. (t. y. 88,1 EUR). Šiuo metu nėra jokios baudos už pinigų grąžinimą
- Jei keičiamasi, jūsų naujasis pirkimas turėtų būti didesnis nei 88,1 EUR
- Šiuo metu nėra taikomos jokios baudos už grąžinamąsias išmokas

**Atsiskaitymo plano rezervavimo pavyzdys:**

- Perkate vienerių metų terminą RI už 10 EUR per mėnesį
- Balandžio 7 d. norite grąžinti pinigus arba pakeisti šį rezervavimą
- Kadangi paskutinis mokėjimas įvyko 7 dienas, gausite (1-7/31) * 10 EUR atgal. (t. y. 7,74 EUR)
- Atšaukti būsimi mokėjimai yra 80 EUR. Šiuo metu nėra jokios baudos už pinigų grąžinimą
- Šis atšaukimas atskaičiuos 87,74 EUR iš jūsų 50 000 EUR grąžinimo limito
- Jei keičiamasi, bendra naujo pirkimo vertė turėtų būti didesnė nei 87,74 EUR

**Rekomenduojami dokumentai**

- [Kaip apdorojamos grąžinimo ir keitimo operacijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- ["Exchange" ir pinigų grąžinimo strategijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)