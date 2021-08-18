---
title: Automatiškai šifruoti Office 365 el. laiškus, siunčiamus į tam tikrus domenus
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318856"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatiškai šifruoti Office 365 el. laiškus, siunčiamus į tam tikrus domenus

1. Administravimo [Exchange pasirinkite pašto](https://outlook.office365.com/ecp/) **srauto > taisykles**. 
2. Spustelėkite **piktogramą Naujas (+),** tada spustelėkite **Taikyti "Office 365" pranešimų šifravimas ir teisių apsaugą laiškams.**
3. Lauke **Pavadinimas** įveskite taisyklės pavadinimą, pvz., Šifruoti laiškus, *siunčiamus contoso.com*.
4. Srityje **Taikyti šią taisyklę, jei** pasirinkite > **domenas** yra . 
5. Įveskite domeno vardą, pvz., **contoso.com**.
6. Spustelėkite **piktogramą Įtraukti (+),** tada spustelėkite **Gerai.**
7. Šalia lauko **Atlikti šį lauką** spustelėkite **Pasirinkti vieną.** 
8. **Išplečiamajame meniu RMS** šablonas pasirinkite Šifruoti , tada spustelėkite **Gerai**.  (Jei nematote šios parinkties, tai reiškia, kad jūsų planas neapima automatinio šifravimo. Tačiau galite jį įtraukti!)
9. Pasirinkite bet kurį pasirinktinį pasirinkimą (iš pasirinktinių pasirinkimų sąrašo, kurį galite atlikti šiuo metu, daugelis iš jų gali būti palikti su numatytuoju paprastumo parametru).
10. Spustelėkite **Įrašyti**.

**Svarbu:** visada galite grįžti ir redaguoti šią taisyklę vėliau.

Daugiau informacijos apie šifravimo taisyklių sukūrimą žr. Pašto srauto taisyklių apibrėžimas [el. laiškams šifruoti Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)