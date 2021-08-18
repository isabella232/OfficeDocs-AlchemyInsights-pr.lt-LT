---
title: IP adreso radus audito žurnale
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902268"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP adreso radus audito žurnale

IP adresas, atitinkantis vartotojo arba administratoriaus atliekamą veiklą, rodomas audito žurnaluose. Kliento informacija taip pat užregistruojama. Štai kaip nustatyti IP adresą:

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras <https://compliance.microsoft.com> , eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Jei matote pranešimą, kad reikia įjungti auditą, eikite į priekį ir įjunkite jį dabar. Jei ši funkcija neįgalinta, ieškos rezultatai negalės gauti duomenų iš ankstesnių datų.

2. Puslapyje **Tikrinimas** patikrinkite, ar pažymėtas **skirtukas** Ieška, tada sukonfigūruokite šiuos parametrus:
   - **Datos ir laiko diapazonas:** laukuose Pradžia ir Pabaiga pasirinkite **datos** **/ laiko diapazoną.**
   - **Veikla:** jei jus domina konkreti veikla, pasirinkite ją iš sąrašo; kitu atveju bus grąžinta **numatytoji reikšmė Rodyti visų** veiklų rezultatus. Atkreipkite dėmesį, kad tam tikros veiklos gali būti negalima pasirinkti; tačiau šie audito elementai bus grąžinti, **jei pasirinkta Rodyti visų veiklų** rezultatus.
   - **Vartotojai:** priimkite tuščią numatytąją reikšmę, kad būtų pateikti rezultatai visiems vartotojams, arba įveskite vieną ar daugiau vartotojų.

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje.

4. Rezultatuose spustelėkite **Filtruoti rezultatus ir** veiklos filtro lauke įveskite **Set-Mailbox.**

5. Pasirinkite audito įrašą rezultatuose, kad atidarytumėte meniu **Išsami** informacija.

Daugiau informacijos žr. [Audito žurnalo ieška norint ištirti bendrąsias palaikymo problemas](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
