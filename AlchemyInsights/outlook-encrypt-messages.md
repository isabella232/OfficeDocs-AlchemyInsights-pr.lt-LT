---
title: S/MIME programoje "Outlook" žiniatinklyje
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666848"
---
# <a name="encrypt-email-messages-in-outlook"></a>Užšifruoti el. laiškus "Outlook"

Office 365 pranešimų šifravimas yra pastatytas ant Microsoft Azure teisių valdymo (Azure RMS), kuris yra Azure informacijos apsaugos dalis. Jei jūsų prenumeratoje yra "Azure" teisių valdymas arba "Azure" informacijos apsauga, **jums nereikia imtis jokių veiksmų, kad įgalintumėte arba suaktyvintumėte** teisių valdymo tarnybą.

Atsižvelgiant į klientų atsiliepimus, mes nebebus įgalinti Exchange pašto srauto taisyklės automatiškai užšifruoti siunčiamų el. laiškų, kuriuose yra tam tikros rūšies slaptą informaciją savo nuomotojo pagal numatytuosius parametrus. Vietoj to, mes pateikti išsamias instrukcijas apie tai, kaip jūs galite padaryti patys. Daugiau informacijos, kaip sukurti transportavimo taisyklę slaptai informacijai užšifruoti, rasite [šiame straipsnyje](https://aka.ms/OmeEtr).

- Jei naudojate "Outlook" internete (anksčiau **OWA**): kurdami el. laišką, tiesiog spustelėkite **apsaugoti** OWA. Tai bus taikoma "neperduoti" leidimo. Spustelėkite **keisti leidimą** ir pasirinkite **šifruoti** , kad užšifruotumėte tik pranešimą.

- Jei naudojate **"Outlook Client"**: siųsti užšifruotą pranešimą iš "Outlook" 2013 arba 2016, arba "Outlook" 2016 for Mac, pasirinkite **parinkčių** > **teisės**, tada pasirinkite norimą apsaugos parinktį.

- Norėdami **automatiškai užšifruoti visus el. laiškus** , nusiųstus tam tikriems gavėjams arba išorinėms partnerių organizacijoms, turite sukurti pašto srauto transportavimo taisyklę "Exchange" administravimo centre. Išsamios instrukcijos pateikiamos [šiame palaikymo straipsnyje](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

