---
title: Pasikartojantis įrenginio įrašas portale
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004162"
---
# <a name="duplicate-device-record-in-the-portal"></a>Pasikartojantis įrenginio įrašas portale

Galite matyti 2 įrenginio įrašus portale, jei įrenginys netinkamai praneša apie bendro valdymo būseną į Konfigūracijos tvarkyklės svetainę. Norėdami patikrinti įrenginio bendro valdymo būseną, peržiūrėkite **bendrai valdomo įrenginio** stulpelį Konfigūracijos tvarkyklės konsolėje. Jei stulpelis nerodomas, galite jį įtraukti dešiniuoju pelės klavišu spustelėdami bet kurią stulpelio antraštę ir pažymėdami jį sąraše.

Bendrai valdoma reikšmė turi būti **Taip**. Jei reikšmė yra **Ne**, atidarykite Konfigūracijos tvarkyklės kliento programą kliento įrenginyje ir skirtuke Bendra pažymėkite ypatybę **Bendras valdymas**.

- Jei reikšmė **Įgalinta**, tai reiškia problemas su kliento ir valdymo taško ryšiu. Peržiūrėkite **CcmMessaging.log** įrenginyje, kad ištirtumėte galimas ryšio triktis.

- Jei reikšmė **Išjungta** ir įrenginys užregistruotas „Intune“, įsitikinkite, kad įrenginys gavo bendro valdymo strategiją peržiūrę **CoManagementHandler. log** įrenginyje.
