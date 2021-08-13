---
title: Kodėl man išjungtas mygtukas Įtraukti biudžetą?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954681"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Kodėl man išjungtas mygtukas Įtraukti biudžetą?

Norėdami sukurti biudžetą, turite turėti vieną iš šių teisių:

- Valdymo grupė, prenumerata, išteklių grupės aprėptis
- Išlaidų valdymo bendraautorių
- Savininkas
- Bendraautorius
- Tik įmonės klientams: registracija, skyrius, paskyros aprėptis
- Registracijos administratorius (nustatykite biudžetą registracijos aprėdoje)
- Skyriaus administratorius (nustatykite biudžetą pagal skyriaus aprėptį)
- Paskyros savininkas (nustatykite biudžetą paskyros aprėdoje)
- Tik moderni kliento sutartis: atsiskaitymo paskyra, atsiskaitymo profilis, sąskaitos faktūros sekcijos aprėptis
- "Azure" prenumeratos kūrėjas

**Sukūriau biudžetą, kai mano dabartinio mėnesio kaina jau buvo per daug biudžeto. Kodėl negaunu įspėjimo?**  
Jei jau viršijote nurodytą išlaidų ribą, kai kuriate biudžetą, kuris nebus įžeidęs. Kai prasidės naujas ciklas, jei pažeisite ribą, tada įspėjimas įeis.

**Kada turėčiau tikėtis gauti įspėjimą, kai viršijau vieną iš mano nustatytų biudžeto įspėjimo slenksčių?**  
Biudžetas vertinamas kas 4 valandas. Užtrunka mažiausiai 8 valandas, kol naudojimo duomenys pasiekia biudžetų sistemą. Atsižvelgiant į tai, įspėjimai gali užtrukti iki 12 valandų, kol viršysite ribą.

**Kodėl mygtukas Pradžios data išjungtas pasirinkus mėnesio arba atsiskaitymo mėnesio nustatymo iš naujo laikotarpį?**  
Biudžetas sulygiuojamas su dabartiniu kalendoriniu mėnesiu arba dabartiniu atsiskaitymo laikotarpiu (tuo atveju, jei pasirenkamas atsiskaitymo mėnuo). Todėl iš anksto užpildome šią reikšmę už jus.

**Kodėl biudžeto kūrimo metu nematau savo išlaidų grafiko?**  
Mums reikia mažiausiai 2 mėnesių išlaidų duomenų, kad galėtume sugeneruoti grafiką, kad galėtume padėti kurti biudžetą.

**Kodėl negaliu nustatyti biudžeto pagal ką tik sukurtą prenumeratą?**  
Sukūrus prenumeratą, duomenys apdorojami per 24–48 valandas prieš nustatant biudžetą pagal ją.

**Biudžeto API ištekliai**

- [Biudžetų API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): pateikia operacijas, skirtas biudžetams kurti ir naujinti. Naudodami biudžeto API, galite nustatyti biudžeto ribą ir sukonfigūruoti kelis įspėjimus, kad jie būtų gesinti artėjant prie šios ribinės vertės. Įspėjimai gali sukelti el. laišką arba "Azure" veiksmų grupę automatizavimui atlikti. Pastaba: šios API filtravimas nesulygiuoja su užklausų API filtravimu / matmenimis.
- [Biudžetų API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)sukurkite biudžetus su didesnėmis nei v1 išlaidų filtravimo galimybėmis. Filtravimas sulygiuoja su mūsų užklausos ir dimensijų API naudojama sutartimi. Tai rekomenduojama biudžetų API, naudojama judėti pirmyn.
- [Matmenys:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)pateikia operacijas, kad gautumėte palaikomus jūsų naudojimo matmenis pagal įvairias aprėptis. Naudodami dimensijų API galite gauti dimensijų, kurios gali būti naudojamos kaip įvestys užklausoms generuoti naudojant užklausos API, sąrašą.
- [Užklausa](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): pateikia operacijas, kad būtų galima gauti agreguotas išlaidų ir naudojimo duomenis pagal jūsų teikiamų užklausų duomenis. Naudodami užklausos API galite nurodyti norimą filtravimą, rūšiavimą ir grupavimą pagal visus galimų dimensijų matmenis (kurie pasiekiami iš dimensijų API).

**Prognozuojamos išlaidos**

**Kodėl išlaidų analizėje nematau savo išlaidų prognozių?**  
Yra kelios priežastys, kodėl išlaidų analizėje gali trūkti prognozės projekcijos, kai kurios iš jų yra tokios:

1. Jei jūsų išlaidų duomenys yra senesni nei 10 dienų, prognozės diagrama nebus įkelta. Modeliui reikia bent 10 dienų naujausių išlaidų duomenų tikslioms prognozėms
2. Jei pasirinkote istorines datas, prognozės diagrama nebus matoma. Pasirinkite datų diapazoną su būsimomis prognozės diagramos, kurią norite rodyti, datomis
3. Jei jūsų paskyroje yra kelios valiutos, prognozės diagramoje bus tik "Visos išlaidos JAV doleriais" projekto išlaidos

**Kodėl nepasikeičia prognozė, kai pakeičiau savo išteklius?**  
Prognozės modeliui reikia kelių dienų, kad būtų galima atsižvelgti į paskyros pakeitimus, o ne iš karto prognozes, pagrįstas išteklių pasikeitimu  
Jei reikia didesnių išteklių padidėjimo arba sumažėjimo veiksmų, modelis šiek tiek ilgiau prisitaikys prie šių pakeitimų, kad būtų galima atsižvelgti į anomalijas

**Kodėl mano prognozė didėja atlikus užsakymą arba įsigius prekyvietę?**  
Prognozės modelyje atsižvelgiama į faktinę kainą ir atskirai neįeisite į naudojimą ir pirkimą. Vienkartinio įsigijimo atveju modelis sumažins prognozes po 10 dienų, kad būtų atsižvelgta į staigų išlaidų padidėjimą

**Noriu matyti vieno matmens prognozes (pvz., Skaitiklis)**  
Šiuo metu prognozė palaiko bendras išlaidų prognozes, o ne atskirus metrus. Taigi, kai dimensija sugrupuota pagal, prognozės bus visų dimensijos elementų sumai

**Rekomenduojami dokumentai**

- [Kas yra "Azure Cost Management"?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Azure Cost Management" geriausia praktika](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Išlaidų ir išlaidų analizė](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Išlaidų tyrimas ir analizė naudojant išlaidų analizę](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Azure Cost Management": kainos](https://azure.microsoft.com/services/cost-management/#pricing)
- [Išlaidų analizės peržiūra](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Vaizdo įrašų mokymo programa: biudžeto kūrimas "Azure" portale](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Būtinos biudžeto peržiūros ir tinkinimo sąlygos](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Biudžetų kūrimas ir valdymas](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatizavimo konfigūravimas naudojant "Azure" veiksmų grupes ir biudžetų API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Naudokite išlaidų įspėjimus, kad stebėtų naudojimą ir išlaidas](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Geriausia išlaidų valdymo praktika](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Mokomieji vaizdo įrašai**

- [Biudžeto kūrimas "Azure" portale](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Išlaidų valdymas naudojant biudžetų API ir veiksmų grupes](https://go.microsoft.com/fwlink/?linkid=2147038)