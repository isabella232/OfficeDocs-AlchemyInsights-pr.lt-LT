---
title: Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip tai padaryti
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988213"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Sužinokite, kas nustato peradresavimą pašto dėžutėje ir kaip tai padaryti

Jei išorinis peradresavimas buvo nustatytas pašto dėžutėje, veikla audituota kaip "cmdlet" Set-Mailbox dalis. Štai kaip rasti veiklą audito žurnale:

1. Eikite į [Office 365 saugos & centrą](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Pasirinkite **Ieškoti** >  **audito žurnalo ieškos**.
    > [!NOTE]
    > Jei matote pranešimą, kad reikia įjungti auditą, eikite į priekį ir įjunkite jį dabar. Jei ši funkcija neįjungta, ieškos rezultatai negalės gauti duomenų iš ankstesnių datų.
1. **Įsitikinkite, kad lauke** Veikla nustatyta rodyti visų **veiklų rezultatus** (numatytasis parametras). Nurodykite datų diapazoną. Nereikia nurodyti vartotojo vardo.
1. Pasirinkite **Ieškoti**. Veikla rodoma dalyje **Rezultatai**.
1. Pasirinkite **Filtruoti** rezultatus , tada lauke Veiklos filtras įveskite **Set-mailbox.**  Taip bus pateikiama visa **set-Mailbox** veikla.
1. Norėdami peržiūrėti išsamią informaciją, pasirinkite veiklą, tada pasirinkite **Daugiau informacijos**. Dalyje **Parametrai** galite matyti peradresavimo el. pašto adresą, kuris buvo nustatytas pašto dėžutėje. Vartotojo **ID nurodo** vartotoją, kuris nustatė išorinį peradresavimą pašto dėžutėje.
Norėdami sužinoti daugiau, [žr. Office 365 žurnalo trikčių šalinimas.](https://go.microsoft.com/fwlink/?linkid=2103944)