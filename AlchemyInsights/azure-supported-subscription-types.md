---
title: Palaikomi prenumeratos tipai
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807973"
---
# <a name="supported-subscription-types"></a>Palaikomi prenumeratos tipai

Peržiūrėkite palaikomų prenumeratos tipus Norėdami tęsti.

[Palaikomi prenumeratos tipai](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Atsiskaitymo nuosavybės perdavimas**

"Azure" portalas kaip atsiskaitymo paskyros, kurioje yra norima perduoti prenumerata, [abonemento administratorius](https://ms.portal.azure.com/)

- **Išlaidų valdymo ir atsiskaitymo** ieška. Pasirinkite **prenumeratos** iš kairės srities. Atsižvelgiant į "Access", gali tekti pasirinkti atsiskaitymo aprėptį ir **prenumeratos** arba "Azure" **prenumeratas** .
- Pasirinkite prenumeratos, kurią norite perkelti, nuosavybę
- Įveskite vartotojo, kuris yra paskyros administratorius, kuris bus naujas prenumeratos savininkas, elektroninio pašto adresą, tada pasirinkite **Siųsti perkėlimo užklausą**
- Vartotojas gauna laišką su nurodymais, kaip peržiūrėti savo perkėlimo užklausą. Norėdami patvirtinti perkėlimo užklausą, vartotojas pasirenka saitą el. laiške ir vadovaujasi nurodymais.

Pastaba: jei persiunčiate savo prenumeratos nuosavybėn vartotojo paskyrą kitame "Azure AD" nuomotojuje, visi [vaidmenimis pagrįsti "Access" valdymo (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) priskyrimai, skirti išteklių prenumeratai, yra visam laikui pašalinti. Tik naujasis savininkas turės prieigą prie prenumeratos išteklių valdymo. Daugiau informacijos ieškokite [vartotojo prenumeratos perdavimas kitam "AZURE AD" nuomotojui](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenumeratos nuosavybės perdavimas**

Prenumeratos nuosavybės perdavimo būtinųjų sąlygų vaidmuo pagal prieigą (RBAC), kad būtų valdomi ištekliai prenumeratoje, praranda prieigą. Daugiau informacijos apie esamos prenumeratos įtraukimą į nuomotoją rasite "Azure [Active Directory" Azure prenumeratos susiejimas arba įtraukimas](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenumeratos perdavimas su esama neapmokėta suma iš dabartinio atsiskaitymo ciklo nebus perkeltas į naują mokėjimo priemonę naujame abonemente. Vienintelė informacija, kurią vartotojai gali naudoti naujoje paskyroje, yra Paskutinė mėnesinė produktų paketą. Likusioji naudojimo ir atsiskaitymo retrospektyva nėra perkeliama su prenumerata.
- "Enterprise" sutarties (EA) prenumeratų atsiskaitymo nuosavybės perdavimas šiuo metu palaikomas įmonės sutarties portale
- Perkeliant kreditus orientuotą prenumeratą, pvz., "Visual Studio", "BizSpark", "Microsoft" partnerių tinklo, naujam vartotojui reikia turėti "Visual Studio"/"Microsoft" partnerių tinklo licenciją, kad priimtumėte perkėlimo užklausą
- Visi ištekliai, pvz., virtualiosios mašinos, diskai ir žiniatinklio svetainės, sėkmingai perkeliami į naująją paskyrą. Šių išteklių gali turėti įtakos kelių nuomotojų prenumeratos perdavimas:

**"Azure AD" domenų tarnybos**

"Azure" raktų skliautai

- " [SQL" susiję vartotojai ir duomenų bazės](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) gali turėti įtakos, ypač jei klientas naudoja "Azure Active Directory" susijusį autentifikavimą
- Galėjo veikti "Azure Active Directory" autentifikavimo sukonfigūruotos **taikomosios programos tarnybos**
- " **Visual Studio" komanda** Tarnybų abonementai, prijungti prie "Azure" prenumeratų, gali laikinai prarasti prieigą, kai yra atšaukta prijungta "Azure" prenumerata

**Rekomenduojami dokumentai**

Veiksmai priėmus atsiskaitymo nuosavybę:

- Norėdami išlaikyti atsiskaitymo nuosavybę, tačiau pakeiskite savo prenumeratos tipą, skaitykite: ["Azure" prenumeratos perjungimas į kitą pasiūlymą](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- ["Visual Studio", "Microsoft" partnerių tinklo (MPN) perkėlimas ir mokėjimas už "dev/Test" prenumeratas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Atsiskaitymo už įmonės sutarties (EA) prenumeratas perdavimas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Perduoti nuosavybės DUK](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Perdavimo nuosavybės problemų šalinimas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)