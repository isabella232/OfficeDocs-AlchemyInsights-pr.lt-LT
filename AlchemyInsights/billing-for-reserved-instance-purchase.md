---
title: Atsiskaitymas už rezervuotą egzempliorių pirkimą
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823163"
---
# <a name="billing-for-reserved-instance-purchase"></a>Atsiskaitymas už rezervuotą egzempliorių pirkimą

Rezervuotųjų egzempliorių pirkimas yra įtraukiamas į mokėjimo metodą, susietą su prenumerata, kurią pasirenkate pirkimo metu. Prenumeratos tipas turi būti įmonės sutartis (pasiūlymo numeris: MS-AZR-0017P), Pay-as-you-go (pasiūlymo numeris: MS-AZR-0003P), "Microsoft" kliento sutartis arba CSP.

- "Enterprise" prenumeratos mokesčiai išskaitomi iš įtraukimo į pinigines įsipareigojimų balansą arba mokami kaip perteklius
- Jei reikia mokėti už prenumeratą, mokesčiai mokami kredito kortelei arba sąskaitos faktūros mokėjimo būdui prenumeratos

**Rezervavimo atšaukimas**

- **Savarankiškas aptarnavimas:** Galite atšaukti arba keistis rezervuotais egzemplioriumi naudodami " [Azure" portalą](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pasirinkite rezervavimą ir spustelėkite grąžinimas arba "Exchange". Turėkite omenyje, kad "Exchange" arba "grąžinamąją išmoką" turite turėti savininko prieigą prie užsakymo tvarkos. Prieiga prie tik rezervavimo neleis jums grąžinti pinigus arba "Exchange". Paprašykite, kad jūsų savininko prieigos prie rezervacijos tvarka būtų suteikta tik rezervavimo užsakymui.
- " **Exchange" strategija:** Galite pakeisti rezervavimą kitoje to paties tipo rezervate – nėra **jokių nuobaudų** dėl užsakymų keitimo. Bendras įsipareigojimas su nauja rezervacija turėtų būti didesnis už pakeistos rezervavimo sumos sumą ir būsimus mėnesinius mokėjimus (jei taikoma)
- **Grąžinimo strategija:** Grąžinimo suma ir atšaukti būsimi mokėjimai negali viršyti $50 000 USD 12 mėnesių tęstinėje lange. **Šiuo metu neapmokestiname jokios baudos** už grąžinamąsias išmokas, tačiau jos gali imti mokestį už būsimus pinigus

**Išimtys:** Savitarnos "Exchange" ir atšaukimo galimybės Galimos JAV vyriausybės įmonės sutarties klientams

- **API/PS/CLI** palaikymas negalimas anuliavimo ir lėšų grąžinimas [savitarnos mainams ir lėšų grąžinimas už "Azure" rezervavimus](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Savitarnos "Exchange" ir atšaukimo galimybės Galimos JAV vyriausybės įmonės sutarties klientams. Kiti JAV vyriausybės prenumeratos tipai, įskaitant Pay-as-you-go ir CSP, yra palaikomi

Sužinokite daugiau: [kaip tvarkomi grąžinimo ir valiutos keitimo sandoriai](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Sužinokite daugiau: " [Exchange" ir pinigų grąžinimo strategijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) kiti klausimai: [lankomų rezervuotų egzempliorių dokumentai](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esamo rezervuotųjų egzempliorių (savitarnos) keitimas**

Galite pakeisti rezervavimą kitoje to paties tipo rezervate. Taip pat galite grąžinti rezervavimą iki $50 000 USD per metus, jei jums jo nebereikia. Savitarnos "Exchange" ir atšaukimo galimybės Galimos JAV vyriausybės įmonės sutarties klientams. Kiti JAV vyriausybės prenumeratos tipai, įskaitant Pay-as-you-go ir CSP, yra palaikomi. Norėdami pakeisti arba grąžinti esamą rezervavimą, turite turėti savininko prieigą prie užsakymo tvarkos.

Toliau aprašyti veiksmai, kaip atlikti operaciją užbaigti operaciją

1. prisijungimas prie " [Azure" portalo](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pasirinkite rezervavimus, kuriuos norite grąžinti ir spustelėkite **Exchange** 2. Pasirinkite VM produktą, kurį norite įsigyti, ir įveskite kiekį. Įsitikinkite, kad naujo pirkimo suma yra didesnė nei grąžinimo suma [nustato tinkamą dydį prieš įsigydami](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. operacijos peržiūra ir užbaigimas

**Rezervuotųjų egzempliorių grąžinimas**

Norėdami grąžinti rezervavimą, eikite į **rezervavimo informaciją** ir spustelėkite **grąžinimas**

**Proporcingoji grąžinamoji išmoka:**

" **Pro-ration" ir minimalūs reikalavimai grąžinamajai išmokai ir mainams** Išankstinių užsakymų pavyzdys:

- Įsigiję vienerių metų terminą RI, skirtą "$120" sausio 1 d.
- Balandžio 7 d., kurį norite grąžinti arba pakeisti šią rezervaciją
- Kadangi rezervavimas buvo gyvas 97 dienoms, gausite (1-97/365) * $120 atgal. (pvz., $88,1). Šiuo metu nėra baudų už grąžinamąsias išmokas
- Jei keistis, jūsų naujas pirkimas turėtų būti didesnis nei $88,1
- Šiuo metu nėra baudos už grąžinamąsias išmokas

**Atsiskaitymo plano rezervavimo pavyzdys:**

- Įsigiję vienerių metų trukmės RI už $10 per mėnesį
- Balandžio 7 d., kurį norite grąžinti arba pakeisti šią rezervaciją
- Po paskutinio apmokėjimo nutiko 7 dienas, gausite (1-7/31) * $10 atgal. (pvz., $7,74)
- Būsimi mokėjimai atšaukti yra $80. Šiuo metu nėra baudų už grąžinamąsias išmokas
- Šis atšaukimas $87,74 iš jūsų "$50 000" grąžinamosios išmokos ribos
- Jei keičiasi, bendra naujo pirkimo vertė turi būti didesnė nei $87,74

**Negalima matyti paskutinio atsiskaitymo laikotarpio sąskaitos faktūros**

Kai kurios galimos priežastys, dėl kurių galite nematyti sąskaitos:

- Jūs turite mėnesinį kredito sumą su jūsų produktų paketą, kurio negavote arba turite nemokamą bandomąją versiją. Sąskaita faktūra sugeneruota tik tada, kai skolingi pinigai
- Mažiau nei 30 dienų nuo dienos, kurią užsiprenumeravote "Azure"
- Sąskaita faktūra dar nėra sugeneruota. Palaukite, kol baigsis atsiskaitymo laikotarpis
- Jei nesate paskyros administratorius, senesnės sąskaitos faktūros gali būti jums neprieinamos

**Sąskaitos atsisiuntimas iš "Azure" portalo (. PDF)**

- Pasirinkite prenumeratą iš "Azure" portalo puslapyje [prenumeratų](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) kaip [vartotojas, turintis prieigą prie sąskaitų faktūrų](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Pasirinkite **sąskaitos faktūros**
- Spustelėkite **atsisiųsti sąskaitą faktūrą** , kad peržiūrėtumėte PDF sąskaitos kopiją. Jei jo **nėra** , Sužinokite, [Kodėl nematau paskutinio atsiskaitymo laikotarpio sąskaitos faktūros?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Sąskaitos gavimas el. paštu (. PDF)**

- Puslapyje [prenumeratos](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) pasirinkite prenumeratą. Spustelėkite **sąskaitos faktūros** ir siųskite savo sąskaitą faktūrą
- Spustelėkite **pasirinkti ir sutikite** su sąlygomis. Turėsite pasirinkti kiekvieną jūsų prenumeratą

Pastaba: jei atlikę šiuos veiksmus negaunate el. laiško, įsitikinkite, kad jūsų [profilio ryšio nuostatose](https://account.windowsazure.com/profile) yra teisingas el. pašto adresas

**Savo naudojimo duomenų atsisiuntimas iš "Azure" portalo**

- Prisijungimas prie " [Azure" abonementų centro](https://account.windowsazure.com/Subscriptions) kaip [abonemento administratorius](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Pasirinkite prenumeratą, kurios sąskaitos faktūros ir naudojimo informacija turėtų būti
- **Atsiskaitymo retrospektyvos** pasirinkimas
- Pasirinkite **Peržiūrėti dabartinį sakinį** , kad matytumėte savo mokesčių sąmatą tuo metu, kai buvo sugeneruota sąmata
- Pasirinkite **atsisiųsti naudojimą** , kad atsisiųstumėte kasdienio naudojimo duomenis kaip CSV failą. Jei matote dvi galimas versijas, atsisiųskite 2 versiją

Kiti klausimai: [apsilankymas rezervuotųjų egzempliorių dokumentuose](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Rekomenduojami dokumentai**

- [Atsiskaitymo pagrindai](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Supratimas, kaip taikoma rezervuota egzemplioriaus nuolaida](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Azure" atsiskaitymo sąskaitos faktūros ir kasdienio naudojimo duomenų atsisiuntimas arba peržiūra](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Supratimas, kaip taikoma rezervuota egzemplioriaus nuolaida](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervuotųjų egzempliorių naudojimas jūsų "Pay-as-you-go" prenumeratoje](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Jūsų įmonės registracijos rezervuotųjų egzempliorių naudojimo supratimas](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Windows" programinės įrangos mokesčiai, neįtraukti į rezervuotus egzempliorius](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Saugomos egzemplioriai partnerio centrinio debesies sprendimų teikėjo (CSP) programoje](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)