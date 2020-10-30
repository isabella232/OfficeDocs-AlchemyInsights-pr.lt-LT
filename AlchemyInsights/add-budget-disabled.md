---
title: Kodėl man išjungtas mygtukas įtraukti biudžetą?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807663"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Kodėl man išjungtas mygtukas įtraukti biudžetą?

Norėdami sukurti biudžetą, turite turėti vieną iš šių teisių:

- Valdymo grupė, prenumerata, išteklių grupių aprėptis
- Išlaidų valdymo bendraautoris
- Savininkas
- Bendraautoriui
- Tik įmonės klientas: registracija, skyrius, paskyrų aprėptis
- Registracijos administratorius (nustatyti biudžetą įtraukimo aprėptyje)
- Skyriaus administratorius (nustatyti biudžetą skyriaus aprėptyje)
- Paskyros savininkas (biudžeto sąskaitos nustatymas)
- Tik moderni kliento sutartis: atsiskaitymo paskyra, Atsiskaitymo profilis, sąskaitos faktūros sekcijų aprėptis
- "Azure" prenumeratos kūrėjas

**Sukūriau biudžetą, kai dabartinio mėnesio savikaina jau buvo per biudžetu. Kodėl negavau perspėjimo?**  
Jei jau viršijote nustatytą išlaidų ribą, kai sukuriate biudžetą, kurio įspėjimas bus ne gaisras. Kai tik prasidės naujas ciklas, jei pažeisite slenkstį, įspėjimas bus ugnies.

**Kada turėčiau tikėtis gauti įspėjimą, kai viršijau vieną iš apibrėžtų biudžeto įspėjimų slenksčių?**  
Biudžetai vertinami kas 4 valandas. Norint pasiekti biudžetų sistemą, naudojimo duomenys užtrunka mažiausiai 8 valandas. Atsižvelgiant į tai, įspėjimai gali užtrukti iki 12 valandų iki gaisro, kai viršijate ribą.

**Kodėl mygtukas pradžios data išjungtas, kai galiu pasirinkti mėnesį arba atsiskaitymo mėnesio nustatymo iš naujo laikotarpį?**  
Biudžetai yra sulygiuoti su dabartiniu kalendoriniu mėnesiu arba dabartiniu atsiskaitymo laikotarpiu (tuo atveju, kai pasirinktas atsiskaitymo mėnuo). Todėl iš anksto užpildykite šią reikšmę.

**Kodėl "Budget" kūrimo patirties nematau savo išlaidų grafiko?**  
Jums reikia mažiausiai 2 mėnesių sąnaudų duomenų, kad galėtume sukurti grafiką, kad galėtume padėti jums sukurti biudžetą.

**Kodėl negaliu nustatyti biudžeto pagal ką tik sukurtą prenumeratą?**  
Sukūrus prenumeratą, duomenys trunka 24-48 valandas, kad būtų apdoroti prieš nustatant biudžetą.

**Biudžeto API ištekliai**

- [Biudžetai API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): pateikia operacijas, skirtas sąmatų kūrimui ir naujinimui. Naudodami sąmatų API, galite nustatyti biudžeto ribą ir konfigūruoti kelis įspėjimus į ugnį, kai priartate prie tos ribos. Įspėjimai gali suaktyvinti el. paštą arba "Azure Action" grupę, kad būtų galima atlikti automatizavimą. Pastaba: šio API filtravimas nesulygiuoja su užklausų API filtravimu/dimensijomis.
- [Biudžetai API V2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): kurti biudžetus su didesnėmis sąnaudų filtravimo galimybėmis nei v1. Filtravimas suderinamas su sutartimi, naudojama mūsų užklausoje ir dimensijų API. Tai rekomenduojama biudžetų API, kad būtų galima naudoti perkėlimą pirmyn.
- [Matmenys](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): pateikia operacijas, kad gautumėte palaikomas naudojimo dimensijas pagal įvairias aprėptis. Naudodami dimensijų API, galite gauti dimensijų sąrašą, kurį galima naudoti kaip įvesties užklausas užklausos API generavimui.
- [Užklausa](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): pateikia operacijas, kad gautumėte kaupiamos kainos ir naudojimo duomenis pagal jūsų pateiktą užklausą. Naudodami užklausų API, galite nurodyti norimą filtravimą, rūšiavimą ir grupavimą visuose galimame dimensijoje (kuri pasiekiama iš dimensijų API).

**Prognozuojamos išlaidos**

**Kodėl išlaidų analizėje nematau savo išlaidų prognozių?**  
Yra kelios priežastys, kodėl prognozės projekcija gali trūkti jums atliekant sąnaudų analizę, kai kurios iš jų yra tokios:

1. Jei jūsų sąnaudų duomenys yra mažesni nei 10 dienų, prognozės struktūra nebus įkeliama. Modeliui reikia bent 10 dienų naujausių sąnaudų duomenis tikslioms projekcijoms
2. Jei pažymėjote istorines datas, prognozės struktūra nebus matoma. Pasirinkite datos intervalą su būsimų datų prognozės rodyklėje, kuri bus rodoma
3. Jei jūsų abonementas turi kelias valiutas, prognozės schemoje bus tik projekto išlaidos "visos išlaidos JAV doleriais"

**Kodėl prognozės nesikeičia, kai aš pakeisiu savo išteklius?**  
Prognozės modeliui reikia poros dienų, kad būtų atsižvelgta į paskyros pakeitimus ir nepadaro tiesioginių prognozių, pagrįstų išteklių pasikeitimu  
Jei reikia didesnių veiksmų, kad būtų padidinti ar sumažinti ištekliai, modelis bus šiek tiek ilgesnis prisitaikyti prie šių pasikeitimų, kad būtų atsižvelgta į anomalijas

**Kodėl mano prognozės padidinimas po to, kai galiu atlikti rezervavimą arba įsigyti "Marketplace"?**  
Prognozės modelis atsižvelgia į jūsų "faktinę kainą" ir neatsižvelgia į naudojimą ir pirkimą atskirai. Po vienkartinio įsigijimo modelis sumažins prognozes po 10 dienų, kad būtų atsižvelgta į staigų išlaidų padidėjimą

**Noriu matyti vieno aspekto prognozę (pvz. Skaitiklis**  
Prognozė šiuo metu palaiko bendrųjų išlaidų prognozes, o ne atskirus skaitiklius. Taigi, kai sugrupuota pagal dimensiją, prognozės bus skirtos visiems dimensijų elementams.

**Rekomenduojami dokumentai**

- [Kas yra "Azure" išlaidų valdymas?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Azure" kainos valdymo geriausios praktikos](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Išlaidų ir išlaidų analizė](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kaštų analizė ir analizavimas](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Azure" kainos valdymas: kainodara](https://azure.microsoft.com/services/cost-management/#pricing)
- [Išlaidų analizės išlaidų peržiūra](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Vaizdo įrašų vadovėlis: "Azure" portalo biudžeto kūrimas](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Biudžetų peržiūros ir tinkinimo būtinųjų sąlygų](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Biudžetų kūrimas ir valdymas](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatizavimo konfigūravimas naudojant "Azure" veiksmų grupes ir biudžetų API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Sąnaudų įspėjimų naudojimas, norint stebėti naudojimą ir išlaidas](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Geriausios praktikos sąnaudų valdymas](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Mokomieji vaizdo įrašai**

- [Sąmatos kūrimas "Azure" portale](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Išlaidų valdymas su biudžetų API ir veiksmų grupėmis](https://go.microsoft.com/fwlink/?linkid=2147038)