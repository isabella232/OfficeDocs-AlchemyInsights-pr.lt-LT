---
title: Darbo diena su skelbimo vartotojo parengimas pereina į sulaikytą būseną
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481879"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Darbo diena su skelbimo vartotojo parengimas pereina į sulaikytą būseną

**Darbo diena su skelbimo vartotojo parengimas patenka į sulaikytą būseną, o AD nėra kuriami jokie vartotojai**

Darbo dienos į skelbimų vartotojo parengimo užduotį atvyko į karantiną ir audito žurnalai rodo eksportavimo triktis su klaidos pranešimo **klaida: OperationsError-SvcErr: įvyko operacijos klaida. Katalogo tarnybai nesukonfigūruota aukštesnioji nuoroda. Todėl katalogų tarnyba negali perduoti klausimų į objektus, esančius už šio miško ribų**. Ši klaida paprastai rodoma, jei "Active Directory" talpyklos OU nustatyta netinkamai arba kyla problemų dėl išraiškos priskyrimo, naudojamo su " **Parentatshed" pavadinimu**.

Pažymėkite žymės langelį numatytoji OU naujiems **vartotojams** . Įsitikinkite, kad jūsų skelbime jau yra nurodyta OU. Jei atributo **Atvaizdelyje naudojate Parentasshedname** , įsitikinkite, kad ji visada įvertinama kaip žinomas talpyklos, esančios skelbimo domene, konteineris. Patikrinkite eksportavimo įvykį audito žurnaluose, kad pamatytumėte sugeneruotą reikšmę.

Išsamesnės informacijos apie darbo dienos konfigūravimą automatiniam parengimas ieškokite straipsnyje [Susipažinkite: darbo dienos konfigūravimas automatiniam vartotojų parengimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

