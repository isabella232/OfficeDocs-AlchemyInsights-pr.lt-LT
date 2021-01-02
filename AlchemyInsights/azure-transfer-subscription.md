---
title: Perduoti „Azure“ atsiskaitymo nuosavybės teises
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
- "6849"
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736886"
---
# <a name="transfer-azure-billing-ownership"></a>Perduoti „Azure“ atsiskaitymo nuosavybės teises

Prisijunkite prie [„Azure“ portalas](https://portal.azure.com/) kaip atsiskaitymo paskyros, kurios prenumeratą norite perduoti, administratorius. Jei nesate tikri, ar esate administratorius, arba jums reikia nustatyti, kas yra, žr. [Nustatyti paskyros atsiskaitymo administratorių](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Ieškokite _Išlaidų valdymas + Atsiskaitymas_.
1. Pasirinkite **Prenumeratos** kairiojoje srityje. Atsižvelgiant į prieigą, gali tekti pasirinkti atsiskaitymo aprėptį ir tada **Prenumeratos** arba **„Azure“ prenumeratos**.
1. Pasirinkite **Perduoti atsiskaitymo nuosavybės teises** prenumeratai, kurią norite perkelti.
1. Įveskite vartotojo, kuris yra paskyros atsiskaitymo administratorius ir bus naujas prenumeratos savininkas, el. pašto adresą ir pasirinkite **siųsti perdavimo užklausą**.
1. Vartotojas gaus el. laišką su instrukcijomis, kaip peržiūrėti jūsų perdavimo užklausą. Norint patvirtinti perdavimo užklausą, vartotojas el. laiške pasirenka nuorodą ir vadovaujasi instrukcijomis.

Atminkite, kad jei perduodate savo prenumeratos atsiskaitymo nuosavybės teisę vartotojo paskyrai kitame „Azure AD“ kliente, visos [vaidmenimis pagrįstas prieigos valdymas (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) prenumeratos išteklių tvarkymo užduotys yra visam laikui pašalinamos. Tik naujas savininkas turės prieigą prie prenumeratos išteklių tvarkymo. Daugiau informacijos apie tai, kaip pakeisti prenumeratos katalogą, žr. [Prenumeratos perdavimas kitam „Azure AD“ nuomininkui priklausančiam vartotojui](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Svarbus poveikis jūsų sąskaitoms faktūroms**_: jei perdavėte „Azure“ prenumeratos atsiskaitymo nuosavybės teisę, jūsų mokesčiai bus imami proporcingai. Turėsite prieigą prie sąskaitų faktūrų kai nurodyta toliau:  

1. Pasirinkite savo prenumeratą [Prenumeratų puslapis](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) „Azure“ portale kaip [vartotojas, turintis prieigą prie sąskaitų faktūrų](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), tuomet pasirinkite **Sąskaitos**.
1. Spustelėkite **Atsisiųsti sąskaitą faktūrą** norėdami peržiūrėti PDF sąskaitos faktūros kopiją. Jei rodoma žinutė _Nepasiekiama_, že. [Kodėl nematau sąskaitos už paskutinį atsiskaitymo laikotarpį?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Taip pat galite peržiūrėti savo kasdienį naudojimą spustelėdami **atsiskaitymo laikotarpis**, kad gautumėte sąskaitos faktūros PDF failą ir išsamaus kasdienio naudojimo failo (.CSV) kopiją. Norėdami gauti daugiau informacijos, žr. [Gaukite sąskaitos faktūros ir naudojimo duomenis](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Rekomenduojami dokumentai**

- [Perduoti „Azure“ prenumeratos atsiskaitymo nuosavybės teises kitai paskyrai](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Apie „Azure“ prenumeratos atsiskaitymo nuosavybės teisių perdavimą](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [„Visual Studio“, „Microsoft“ partnerių tinklo (MPN) ir einamųjų įmokų („Pay as you go“) Kūrėjų / Testavimo prenumeratų perdavimas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Nuosavybės teisių perdavimo DUK](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Pašalinti nuosavybės teisių perdavimo problemas](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
