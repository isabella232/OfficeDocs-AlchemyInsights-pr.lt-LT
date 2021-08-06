---
title: Darbo diena į AD vartotojo parengimą patenka į sulaikymo būseną
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036500"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Darbo diena į AD vartotojo parengimą patenka į sulaikymo būseną

**Darbo diena į AD vartotojo parengimą patenka į sulaikymo būseną ir jokie vartotojai nėra sukuriami AD**

Darbo diena su AD vartotojo parengimo užduotimi perėjo į sulaikymo būseną, o audito žurnaluose rodomi eksportavimo nesėkmių įvykiai su klaidos pranešimu **Klaida: OperationsError-SvcErr: įvyko operacijos klaida. Katalogų tarnybai nebuvo sukonfigūruota jokia geresnė nuoroda. Todėl katalogų tarnyba negali pateikti referalų objektams už šio miško** ribų. Ši klaida paprastai rodoma, jei "Active Directory" konteineris OU nustatytas netinkamai arba yra problemų su reiškinio susiejimu, naudojamu **parentDistinguishedName**.

Patikrinkite rašybos klaidų **parametrą Numatytasis** OU naujiems vartotojams. Įsitikinkite, kad nurodytas OU jau yra jūsų AD. Jei atributų **susiejime naudojate parentDistinguishedName,** įsitikinkite, kad jis visada įvertina žinomą konteinerį AD domene. Patikrinkite įvykį Eksportuoti audito žurnaluose, kad pamatytumėte sugeneruotą reikšmę.

Daugiau informacijos apie automatinio parengimo darbo dienos konfigūravimą žr. [Vadovėlis: Darbo dienos konfigūravimas automatiniam vartotojų parengimui](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

