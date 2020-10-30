---
title: Rezervavimo atšaukimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807996"
---
# <a name="cancelling-reservation"></a>Rezervavimo atšaukimas

- **Savarankiškas aptarnavimas:** Galite atšaukti arba keistis rezervuotais egzemplioriumi naudodami " [Azure" portalą](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pasirinkite rezervavimą ir spustelėkite grąžinimas arba "Exchange". Turėkite omenyje, kad "Exchange" arba "grąžinamąją išmoką" turite turėti savininko prieigą prie užsakymo tvarkos. Prieiga prie tik rezervavimo neleis jums grąžinti pinigus arba "Exchange". Paprašykite, kad jūsų savininko prieigos prie rezervacijos tvarka būtų suteikta tik rezervavimo užsakymui.
- " **Exchange" strategija:** Galite pakeisti rezervavimą kitoje to paties tipo rezervate – nėra **jokių nuobaudų** dėl užsakymų keitimo. Bendras įsipareigojimas su nauja rezervacija turėtų būti didesnis už pakeistos rezervavimo sumos sumą ir būsimus mėnesinius mokėjimus (jei taikoma)
- **Grąžinimo strategija:** Grąžinimo suma ir atšaukti būsimi mokėjimai negali viršyti $50 000 USD 12 mėnesių tęstinėje lange. **Šiuo metu neapmokestiname jokios baudos** už grąžinamąsias išmokas, tačiau jos gali imti mokestį už būsimus pinigus  
    **Išimtys:** Savitarnos "Exchange" ir atšaukimo galimybės Galimos JAV vyriausybės įmonės sutarties klientams
- **API/PS/CLI** palaikymas negalimas anuliavimo ir lėšų grąžinimas [savitarnos mainams ir lėšų grąžinimas už "Azure" rezervavimus](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Savitarnos "Exchange" ir atšaukimo galimybės Galimos JAV vyriausybės įmonės sutarties klientams. Kiti JAV vyriausybės prenumeratos tipai, įskaitant Pay-as-you-go ir CSP, yra palaikomi

Sužinokite daugiau: [kaip apdorojamos grąžinimo ir keitimo operacijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Sužinokite daugiau: " [Exchange" ir pinigų grąžinimo strategijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Kiti klausimai: [apsilankymas rezervuotųjų egzempliorių dokumentuose](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Esamo rezervuotųjų egzempliorių (savitarnos) keitimas**

Galite pakeisti rezervavimą kitoje to paties tipo rezervate. Taip pat galite grąžinti rezervavimą iki $50 000 USD per metus, jei jums jo nebereikia. Savitarnos "Exchange" ir atšaukimo galimybės Galimos JAV vyriausybės įmonės sutarties klientams. Kiti JAV vyriausybės prenumeratos tipai, įskaitant Pay-as-you-go ir CSP, yra palaikomi. Norėdami pakeisti arba grąžinti esamą rezervavimą, turite turėti savininko prieigą prie užsakymo tvarkos.

Toliau aprašyti veiksmai, kaip atlikti operaciją užbaigti operaciją

1. Prisijungimas prie " [Azure" portalo](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pasirinkite norimas grąžinti išlygas ir spustelėkite " **Exchange** "
2. Pasirinkite VM produktą, kurį norite įsigyti, ir įveskite kiekį. Įsitikinkite, kad naujo pirkimo suma yra didesnė nei grąžinimo suma [nustato tinkamą dydį prieš įsigydami](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Operacijos peržiūra ir užbaigimas

**Rezervuotųjų egzempliorių grąžinimas**

Norėdami grąžinti rezervavimą, eikite į **rezervavimo informaciją** ir spustelėkite **grąžinimas**

**Proporcingoji grąžinamoji išmoka:**

**"Pro-ration" ir minimalūs reikalavimai grąžinamajai išmokai ir mainams**  
Išankstinių užsakymų pavyzdys:

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

**Rekomenduojami dokumentai**

- [Kaip apdorojamos grąžinimo ir keitimo operacijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- ["Exchange" ir pinigų grąžinimo strategijos](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)