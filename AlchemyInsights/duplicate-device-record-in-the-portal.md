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
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814524"
---
# <a name="duplicate-device-record-in-the-portal"></a>Pasikartojantis įrenginio įrašas portale

Galite matyti 2 įrenginio įrašus portale, jei įrenginys netinkamai praneša apie bendro valdymo būseną į Konfigūracijos tvarkyklės svetainę. Norėdami patikrinti įrenginio bendro valdymo būseną, peržiūrėkite **bendrai valdomo įrenginio** stulpelį Konfigūracijos tvarkyklės konsolėje. Jei stulpelis nerodomas, galite jį įtraukti dešiniuoju pelės klavišu spustelėdami bet kurią stulpelio antraštę ir pažymėdami jį sąraše.

Bendrai valdoma reikšmė turi būti **Taip**. Jei reikšmė yra **Ne**, atidarykite Konfigūracijos tvarkyklės kliento programą kliento įrenginyje ir skirtuke Bendra pažymėkite ypatybę **Bendras valdymas**.

- Jei reikšmė **Įgalinta**, tai reiškia problemas su kliento ir valdymo taško ryšiu. Peržiūrėkite **CcmMessaging.log** įrenginyje, kad ištirtumėte galimas ryšio triktis.

- Jei reikšmė **Išjungta** ir įrenginys užregistruotas „Intune“, įsitikinkite, kad įrenginys gavo bendro valdymo strategiją peržiūrę **CoManagementHandler. log** įrenginyje.
