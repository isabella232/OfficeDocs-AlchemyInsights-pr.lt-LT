---
title: Panaikintų įvykių audito žurnalų skaitymas
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324741"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Panaikintų įvykių audito žurnalų skaitymas

Štai kaip tai padaryti:

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras , <https://compliance.microsoft.com> eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> , eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://security.microsoft.com/auditlogsearch> .

    **Pastaba:** jei matote pranešimą, kad reikia įjungti funkciją, eikite į priekį ir įjunkite ją dabar. Jei funkcija neįjungta, ieškos rezultatai negalės gauti duomenų iš ankstesnių datų.

2. Audito **puslapio** skirtuke **Ieška** sukonfigūruokite šiuos parametrus:
   - **Datos ir laiko diapazonas:** laukuose Pradžia ir Pabaiga pasirinkite **datos** / **laiko diapazoną.**
   - **Veikla**: Exchange **pašto dėžutės veiklą** ir pasirinkite šias reikšmes:
     - **Panaikinti laiškai iš aplanko Panaikinti elementai**
     - **Perkelti laiškai į aplanką Panaikinti elementai**

       Kai baigsite, spustelėkite už srities ribų, kad minimizuoti **sritį** Veikla.

   - **Vartotojai:** priimkite tuščią numatytąją reikšmę, kad būtų pateikti rezultatai visiems vartotojams, arba įveskite vieną ar daugiau vartotojų.

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje.

4. Pasirinkite veiklą rezultatuose, kad atidarytumėte išsamios informacijos iškelia į lauką. Lauke **AffectedItems** rodoma papildoma informacija apie panaikintą elementą, pvz., temos eilutė ir elemento vieta, kai jis buvo panaikintas.

   **Pastaba:** negalite atkurti panaikintų elementų naudodami audito žurnalo funkciją. Norėdami atkurti panaikintus elementus, [žr. Panaikintų el. laiškų atkūrimas internetinė "Outlook"](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Daugiau informacijos žr. [Audito žurnalo ieška norint ištirti bendrąsias palaikymo problemas](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
