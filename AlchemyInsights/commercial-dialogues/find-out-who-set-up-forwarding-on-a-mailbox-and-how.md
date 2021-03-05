---
title: Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482302"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip

Jei išorinis peradresavimas buvo nustatytas pašto dėžutėje, veikla tikrinama kaip Set-Mailbox cmdlet dalis. Toliau aprašyta, kaip galite sužinoti veiklos auditą:

1. Eikite į " [Office 365" saugos & atitikties centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Pasirinkite **ieškos** >  **audito žurnalų ieška**.
    > [!NOTE]
    > Jei matote pranešimą, kad turite įjungti auditą, eikite į priekį ir įjunkite jį dabar. Jei ši funkcija nėra įjungta, ieškos rezultatai negalės ištraukti ankstesnių datų duomenų.
1. Įsitikinkite, kad lauke **veikla** nustatyta **Rodyti visų veiklų rezultatus** (numatytasis parametras). Nurodo datų intervalą. Jums nereikia įvesti vartotojo vardo.
1. Pasirinkite **Ieškoti**. Veikla rodoma dalyje **rezultatai**.
1. Pasirinkite **filtruoti rezultatus**, tada lauke **veiklos** filtras įveskite **Set-Mailbox** . Tai pateikia visas **nustatytas pašto dėžutės** veiklas.
1. Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite **daugiau informacijos**. Dalyje **Parametrai** galite matyti peradresavimo el. pašto adresą, kuris buvo nustatytas pašto dėžutėje. **UserID** vaizduoja vartotoją, kuris nustatė išorinį peradresavimą pašto dėžutėje.
Norėdami sužinoti daugiau, skaitykite " [Office 365" audito žurnalų ieška, kad išspręstumėte įprastus scenarijus](https://go.microsoft.com/fwlink/?linkid=2103944).