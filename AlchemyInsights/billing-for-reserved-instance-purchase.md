---
title: Atsiskaitymas už rezervuotąjį egzempliorių pirkimą
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820330"
---
# <a name="billing-for-reserved-instance-purchase"></a>Atsiskaitymas už rezervuotąjį egzempliorių pirkimą

Rezervuotųjų egzempliorių įsigijimas apmokestinamas mokėjimo metodu, susietomis su prenumerata, kurią pasirenkate pirkimo metu. Prenumeratos tipas turi būti įmonės sutartis (pasiūlymo numeris: MS-AZR-0017P), "Pay-As-You-Go" (pasiūlymo numeris: MS-AZR-0003P), "Microsoft" klientų sutartis arba CSP.

- Už įmonės prenumeratą mokesčiai atimami iš registracijos piniginio įsipareigojimo likučio arba apmokestinami kaip perpildai
- Už "Pay-As-You-Go" prenumeratą mokesčiai išrašomi iš kredito kortelės arba sąskaitos faktūros mokėjimo būdo prenumeratoje

**Rezervavimo atšaukimas**

- **Savitarnos paslauga:** Rezervuotąjį egzempliorių galite atšaukti arba pakeisti patys naudodami ["Azure" portalą.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Pasirinkite rezervavimą ir spustelėkite grąžinti arba keisti. Atkreipkite dėmesį, kad turite turėti savininko prieigą rezervavimo užsakyme, kad galėtumėte pakeisti arba grąžinti pinigus. Prieiga prie tik rezervavimo neleis jums grąžinti pinigų arba pakeisti. Paprašykite rezervavimo užsakymo savininko suteikti jums savininko prieigą prie rezervavimo užsakymo
- **"Exchange" strategija:** Galite pakeisti kito to paties tipo rezervavimo rezervavimą – už **rezervavimo mainus nėra** jokių baudos. Bendras įsipareigojimas su nauja rezervacija turėtų būti didesnis už valiutos keitimo rezervavimo grąžinimo sumą ir būsimus mėnesinius mokėjimus (jei taikoma)
- **Grąžinimo strategija:** Pinigų grąžinimo ir atšauktų būsimų mokėjimų suma negali viršyti 50 000 JAV dolerių 12 mėnesių einamojo laikotarpio lange. Šiuo metu **neįeisime jokių baudos už pinigų** grąžinimą, bet galėtume ją apmokestinti už būsimas grąžinamąsias išmokas

**Išimtys:** "Us Government Enterprise Agreement" klientams negalimas apsikeitimas savitarnos paslaugomis ir atšaukimo galimybės

- **API / PS / CLI** palaikymas negalimas atšaukimo ir pinigų grąžinimo savitarnos mainams ir [pinigų grąžinimui už "Azure Reservations"](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- "Us Government Enterprise Agreement" klientams negalimas apsikeitimas savitarnos paslaugomis ir atšaukimo galimybė. Palaikomi kiti JAV vyriausybės prenumeratos tipai, įskaitant "Pay-As-You-Go" ir CSP

Sužinokite daugiau : [Kaip apdorojamos grąžinimo ir keitimo](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) operacijos Sužinokite daugiau: ["Exchange" ir pinigų grąžinimo strategijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Kiti klausimai: apsilankykite [rezervuotųjų egzempliorių keiti](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange an existing reserved instance (Self-service)**

Galite pakeisti kito to paties tipo rezervavimo rezervavimą. Be to, jei jums jo nebereikia, galite grąžinti iki 50 000 JAV dolerių per metus. "Us Government Enterprise Agreement" klientams negalimas apsikeitimas savitarnos paslaugomis ir atšaukimo galimybė. Palaikomi kiti JAV vyriausybės prenumeratos tipai, įskaitant "Pay-As-You-Go" ir CSP. Turite turėti savininko prieigą rezervavimo užsakyme, kad galėtumėte pakeisti esamą rezervavimą arba jį grąžinti.

Toliau nurodyti veiksmai padės atlikti operaciją

1.Prisijunkite prie ["Azure" portalo](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pasirinkite rezervavimus, kuriuos norite grąžinti, ir spustelėkite **"Exchange** 2". Pasirinkite VM produktą, kurį norite įsigyti, ir įveskite kiekį. Įsitikinkite, kad nauja pirkimo suma yra didesnė už grąžinamą sumą [Nustatykite tinkamą dydį prieš pirkdami](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Peržiūrėkite ir užbaikite operaciją

**Rezervuotųjų egzempliorių grąžinimas**

Norėdami grąžinti rezervaciją, eikite į **Išsami rezervavimo informacija** ir spustelėkite **Grąžinti**

**Pro-rated refund:**

**Grąžinimo ir keitimo reikalavimo** pavyzdžiai ir minimalūs reikalavimai Išankstinio rezervavimo pavyzdys:

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

**Nepavyko matyti sąskaitos faktūros už paskutinį atsiskaitymo laikotarpį**

Kai kurios galimos priežastys, dėl kurių gali būti nematote sąskaitos faktūros:

- Turite mėnesinę kredito sumą su prenumerata, kurios neviršijote arba turite nemokamą bandomąją versiją. Sąskaita faktūra sugeneruojama tik tada, kai esate skolingi pinigai
- Tai mažiau nei 30 dienų nuo tos dienos, kai prenumeravote "Azure"
- Sąskaita faktūra dar nesugeneruota. Palaukite, kol baigsis atsiskaitymo laikotarpis
- Jei esate ne paskyros administratorius, senesnės sąskaitos faktūros gali būti jums negalimos

**Sąskaitos faktūros atsisiuntimas iš "Azure" portalo (.pdf)**

- Prenumeratos pasirinkimas iš ["Azure"](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) portalo prenumeratos puslapio kaip [vartotojas, kuris turi prieigą prie sąskaitų faktūrų](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Pasirinkite **Sąskaitos faktūros**
- Spustelėkite **Atsisiųsti sąskaitą faktūrą,** kad būtų galima peržiūrėti PDF sąskaitos faktūros kopiją. Jei jame **nurodyta Nėra**, [žr. Kodėl nematau](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) sąskaitos faktūros už paskutinį atsiskaitymo laikotarpį?

**Gaukite sąskaitą faktūrą el. paštu (.pdf)**

- Pasirinkite prenumeratą [puslapyje Prenumeratos.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Spustelėkite **Sąskaitos faktūros, tada el.** paštas mano sąskaita faktūra
- Spustelėkite **Pasirinkti ir** sutikite su sąlygomis. Turėsite pasirinkti kiekvieną prenumeratą, kurią turite

Pastaba: jei atlikę šiuos veiksmus negausite el. laiško, įsitikinkite, kad jūsų el. pašto adresas [teisingas jūsų profilio ryšių nuostatose](https://account.windowsazure.com/profile)

**Naudojimo duomenų atsisiuntimas iš "Azure" portalo**

- Prisijungimas prie ["Azure" paskyros centro](https://account.windowsazure.com/Subscriptions) kaip [paskyros administratorius](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Pasirinkite prenumeratą, kurios sąskaitos faktūros ir naudojimo informaciją norite gauti
- Pasirinkite **Atsiskaitymo retrospektyva**
- Pasirinkite **Peržiūrėti dabartinį sakinį,** kad pamatytumėte savo mokesčių įvertinimą tuo metu, kai buvo sugeneruotas įvertinimas
- Pasirinkite **Atsisiųsti naudojimą,** kad atsisiųstumėte kasdienio naudojimo duomenis kaip CSV failą. Jei matote dvi versijas, atsisiųskite 2 versiją

Kiti klausimai: [aplankykite rezervuotųjų egzempliorių dokumentus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Rekomenduojami dokumentai**

- [Atsiskaitymo pagrindai](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Supraskite, kaip taikoma rezervuotųjų egzempliorių nuolaida](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Azure" atsiskaitymo sąskaitos faktūros ir kasdienio naudojimo duomenų atsisiuntimas arba rodinys](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Supraskite, kaip taikoma rezervuotųjų egzempliorių nuolaida](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Pay-As-You-Go" prenumeratos rezervuotųjų egzempliorių naudojimo supratimas](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Enterprise" registracijos rezervuotųjų egzempliorių naudojimo supratimas](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Windows" programinės įrangos išlaidos, neįtrauktos į rezervuotųjų egzempliorių](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervuotieji egzemplioriai partnerių centrinio debesies sprendimų teikėjo (CSP) programoje](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)