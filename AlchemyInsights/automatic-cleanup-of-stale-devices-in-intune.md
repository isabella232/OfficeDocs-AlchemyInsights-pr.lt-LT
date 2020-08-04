---
title: Automatinis valymas pasenusių prietaisų Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555224"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatinis valymas pasenusių prietaisų Intune

Intune leidžia administratoriui konfigūruoti laiko intervalą tarp 90 ir 270 dienų, po kurio pasenusi prietaisai pašalinami iš tarnybos. Šis parametras yra visos organizacijos ir kai aktyvuota įsigalioja iš karto. Visi įrenginiai, nepažymėti intune serveryje ilgiau nei parametras yra visam laikui panaikinti.

**Pastaba** Šis valymo veiksmas gali būti taikomas tik MDM įrenginio objektams. EAS neįtraukiami tik įrenginio objektai.

Jei norite gauti papildomos informacijos apie tai, kada įrenginys tampa tinkamas naikinti pagal įrenginio valymo nustatymą ir jo būseną:

Nustatymas: **Ištrinti įrenginius po paskutinio įregistravimo datos: Taip (tam tikra vertė (N) nurodytomis dienomis)**

- Pagal parametre sukonfigūruotą reikšmę (N), "Intune" tarnyba panaikina įrenginį nurodytomis dienomis po paskutinio sėkmingai čekio.

Nustatymas: **ištrinti įrenginius po paskutinės registracijos datos: Ne**

- Praėjus 180 dienų nuo įrenginio sertifikato galiojimo pabaigos ir jis neatnaujinamas, įrenginys panaikinamas.

**Pastaba** Abiem atvejais įrenginys turi būti sėkmingai užregistruotas Intune. Registracija įvyksta per pirmąjį įrenginį checkin su Intune paslauga.

Jei įrenginys sėkmingai užregistruoja "Intune", bet netaia ir neužregistravo "Intune", įrenginys panaikinamas praėjus 270 dienų po registracijos. (90 dienų, kad pažymėtumėte įrenginį kaip atšauktą, o tada dar 180 dienų įrašui panaikinti.)

Šiuo metu "Intune" konsolėje nėra mechanizmo, skirto nustatyti įrenginio sertifikavimo galiojimo datą bet kuriam įrenginiui.