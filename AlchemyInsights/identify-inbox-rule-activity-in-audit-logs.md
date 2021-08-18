---
title: Aplanko Gauta taisyklės veiklos tikrinimas audito žurnaluose
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331131"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Aplanko Gauta taisyklės veiklos tikrinimas audito žurnaluose

Galite naudoti audito žurnalo iešką dalyje "Microsoft 365" atitikties centras aplanko Gauta taisyklės įvykius (aplanko Gauta taisyklių kūrimas, modifikavimas ir naikinimas).

1. Atlikite vieną iš šių veiksmų:
   - Lauke "Microsoft 365" atitikties centras <https://compliance.microsoft.com> , eikite į **Sprendimų** \> **auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://compliance.microsoft.com/auditlogsearch> .
   - ""Microsoft 365" sargyba portale <https://security.microsoft.com> eikite į **Auditas**. Arba, norėdami pereiti tiesiai į **audito puslapį,** naudokite <https://security.microsoft.com/auditlogsearch> .

2. Audito **puslapio** skirtuke **Ieška** sukonfigūruokite šiuos parametrus:
   - **Datos ir laiko diapazonas:** laukuose Pradžia ir Pabaiga pasirinkite **datos** / **laiko diapazoną.**
   - **Veikla**: pasirinkite vieną ar daugiau iš šių reikšmių:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Aplanko Gauta taisyklių naujinimas iš Outlook kliento**

3. Kai baigsite, spustelėkite **Ieškoti**. Veikla rodoma naujame audito **ieškos** puslapyje.

4. Pasirinkite veiklą rezultatuose, kad atidarytumėte išsamios informacijos iškelia į lauką. Informacija apie aplanko Gauta taisyklės parametrus rodoma **lauke** Parametrai.

Daugiau informacijos žr. [Nustatymas, ar vartotojas sukūrė aplanko Gauta taisyklę](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
