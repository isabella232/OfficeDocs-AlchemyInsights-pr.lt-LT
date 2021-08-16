---
title: Palaikomų prenumeratų tipai
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072168"
---
# <a name="supported-subscription-types"></a>Palaikomų prenumeratų tipai

Norėdami tęsti, peržiūrėkite palaikomų prenumeratų tipus.

[Palaikomų prenumeratų tipai](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Atsiskaitymo nuosavybės teisių perdavimas**

„Azure“ portalas kaip atsiskaitymo paskyros, kurioje yra prenumerata, kurią norite perkelti, [paskyros administratorius](https://ms.portal.azure.com/).

- Ieškokite dalies **Išlaidų valdymas + Atsiskaitymas**. Pasirinkite **Prenumeratos** kairiojoje srityje. Atsižvelgiant į prieigą, gali tekti pasirinkti atsiskaitymo aprėptį ir tada **Prenumeratos** arba **„Azure“ prenumeratos**.
- Pasirinkite Perduoti atsiskaitymo nuosavybės teises prenumeratai, kurią norite perkelti
- Įveskite vartotojo, kuris yra paskyros atsiskaitymo administratorius ir bus naujas prenumeratos savininkas, el. pašto adresą ir pasirinkite **siųsti perdavimo užklausą**
- Vartotojas gaus el. laišką su instrukcijomis, kaip peržiūrėti jūsų perdavimo užklausą. Norint patvirtinti perdavimo užklausą, vartotojas el. laiške pasirenka nuorodą ir vadovaujasi instrukcijomis.

Pastaba: jei perduodate savo prenumeratos atsiskaitymo nuosavybės teisę vartotojo paskyrai kitame „Azure AD“ kliente, visos [vaidmenimis pagrįstas prieigos valdymas (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) prenumeratos išteklių tvarkymo užduotys yra visam laikui pašalinamos. Tik naujas savininkas turės prieigą prie prenumeratos išteklių tvarkymo. Daugiau informacijos, žr. [Prenumeratos perdavimas kitam „Azure AD“ nuomininkui priklausančiam vartotojui](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenumeratos nuosavybės perdavimas**

Prenumeratos nuosavybės perdavimas iš anksto reikalauja vaidmeniu paremtos prieigos (RBAC), kad galėtų valdyti išteklius, jei prenumeratos praras prieigą. Daugiau informacijos apie esamos prenumeratos įtraukimą į nuomotoją, žr. [„Azure“ paskyros susiejimas su arba įtraukimas į „Azure Active Directory“](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenumeratos perdavimas su esamu likučiu iš dabartinio atsiskaitymo ciklo nebus perkeltas į naująjį mokėjimo instrumentą naujojoje paskyroje. Vienintelė informacija, kuri bus pasiekiama vartotojams naujojoje paskyroje bus praėjusio mėnesio prenumeratos kaina. Likusi vartojimo ir atsiskaitymo istorija su prenumerata neperkeliama.
- Korporatyvinės sutarties (EA) prenumeratų atsiskaitymo nuosavybės perdavimas šiuo metu palaikomas tik korporatyvinės sutarties portale
- Tokios į kreditą orientuotos prenumeratos, kaip „Visual Studio“, „BizSpark“, „Microsoft“ partnerių tinklo perdavimas naujam vartotojui reikalauja turėti „Visual Studio“ / „Microsoft“ partnerių tinklo licenciją, kad būtų galima priimti perdavimo prašymą
- Visi ištekliai, pvz. virtualiosios mašinos, diskai ir svetainės į naująją paskyrą perkeliami sėkmingai. Toliau pateikti ištekliai gali būti paveikti prenumeratos perkėlimo iš vieno nuomotojo į kitą metu:

**„Azure AD“ domeno paslaugos**

„Azure Key Vault“

- [Su SQL susiję vartotojai ir duomenų bazės](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) gali būti paveikti, ypač tuo atveju, jeigu klientas naudoja su „Azure Active Directory“ susijusią autentifikaciją
- **Programų paslaugos** sukonfigūruotos naudojant „Azure Active Directory“ gali būti paveiktos
- **„Visual Studio Team“** paslaugų paskyros prijungtos prie „Azure“ prenumeratų gali laikinai prarasti prieigą, kai prijungta „Azure“ paskyra atšaukiama

**Rekomenduojami dokumentai**

Veiksmai, priėmus atsiskaitymo nuosavybę:

- Norėdami išlaikyti atsiskaitymo nuosavybę, bet pakeisti savo prenumeratos tipą, žr. [Keisti „Azure“ prenumeratą į kitą pasiūlymą](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [„Visual Studio“, „Microsoft“ partnerių tinklo (MPN) ir einamųjų įmokų („Pay as you go“) Kūrėjų / Testavimo prenumeratų perdavimas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Korporatyvinės sutarties (EA) prenumeratų atsiskaitymo nuosavybės perdavimas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Nuosavybės teisių perdavimo DUK](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Pašalinti nuosavybės teisių perdavimo problemas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)