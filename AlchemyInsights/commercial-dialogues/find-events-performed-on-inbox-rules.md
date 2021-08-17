---
title: Įvykių, atliekamų pagal aplanko Gauta taisykles, radimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313507"
---
# <a name="find-events-performed-on-inbox-rules"></a>Įvykių, atliekamų pagal aplanko Gauta taisykles, radimas

Kai kuriamos, keičiamos arba panaikinamos aplanko Gauta taisyklės, įvykiai įrašomi audito žurnale. Štai kaip juos peržiūrėti:

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras , <https://compliance.microsoft.com> eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> , eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://security.microsoft.com/auditlogsearch> .

    **Pastaba:** jei matote pranešimą, kad reikia įjungti auditą, eikite į priekį ir įjunkite jį dabar. Jei ši funkcija neįjungta, ieškos rezultatai negalės gauti duomenų iš ankstesnių datų.
1. Pasirinkite lauką Veikla ir raskite Exchange pašto dėžutės veiklą, tada pasirinkite New-InboxRule Aplanko Gauta taisyklę iš Outlook Web App. Kai baigsite, spustelėkite už srities ribų, kad minimizuoti sritį Veikla.
1. Nurodykite datų diapazoną, tada lauke Vartotojai pasirinkite vartotojo vardą, kurį norite ištirti. Vienu metu galite pasirinkti daugiau nei vieną vartotoją.
1. Pasirinkite Ieškoti. Veikla rodoma dalyje Rezultatai.
1. Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite Daugiau informacijos. Dalyje Parametrai galite matyti taisyklės pavadinimą, sąlygų rinkinį ir veiksmus, kurių ši taisyklė imsis.

2. Audito **puslapio** skirtuke **Ieška** sukonfigūruokite šiuos parametrus:
   - **Datos ir laiko diapazonas:** laukuose Pradžia ir Pabaiga pasirinkite **datos** / **laiko diapazoną.**
   - **Veikla:** pasirinkite **Naujas aplankas Gauta Taisyklė Aplanko Gauta taisyklės kūrimas iš Outlook Web App**

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje.

4. Pasirinkite veiklą rezultatuose, kad atidarytumėte išsamios informacijos iškelia į lauką. Dalyje **Parametrai** galite matyti taisyklės pavadinimą, sąlygų rinkinį ir veiksmus, kurių ši taisyklė imsis.

Norėdami sužinoti daugiau, [žr. Audito žurnalo ieška, kad ištirtumėte bendrąsias palaikymo problemas.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
