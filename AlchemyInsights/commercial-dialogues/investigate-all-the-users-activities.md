---
title: Visų vartotojų veiklų tyrimą
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332351"
---
# <a name="investigate-all-the-users-activities"></a>Visų vartotojų veiklų tyrimą

Štai kaip tai padaryti:

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras , <https://compliance.microsoft.com> eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> , eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://security.microsoft.com/auditlogsearch> .

    **Pastaba:** jei matote pranešimą, kad reikia įjungti funkciją, eikite į priekį ir įjunkite ją dabar. Jei funkcija neįjungta, ieškos rezultatai negalės gauti duomenų iš ankstesnių datų.

2. Audito **puslapio** skirtuke **Ieška** sukonfigūruokite šiuos parametrus:
   - **Datos ir laiko diapazonas:** laukuose Pradžia ir Pabaiga pasirinkite **datos** / **laiko diapazoną.**
   - **Veikla:** jei jus domina konkreti veikla, pasirinkite ją iš sąrašo; kitu atveju numatytoji reikšmė **Rodyti visų veiklų rezultatus grąžina** visas veiklas.
   - **Vartotojai:** priimkite tuščią numatytąją reikšmę, kad būtų pateikti rezultatai visiems vartotojams, arba įveskite vieną ar daugiau vartotojų.

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje. Matysite IP **adresą**, **Vartotojo** ir **Veiklos** pavadinimą.

4. Norėdami atsisiųsti rezultatus, pasirinkite **Eksportuoti atsisiųsti** \> **visus rezultatus**.

5. Pasirinkite veiklą rezultatuose, kad atidarytumėte išsamios informacijos iškelia į lauką.

Norėdami sužinoti daugiau, [žr. Audito žurnalo ieška, kad ištirtumėte bendrąsias palaikymo problemas.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
