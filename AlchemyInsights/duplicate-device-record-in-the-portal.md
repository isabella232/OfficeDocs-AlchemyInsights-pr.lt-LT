---
title: Pasikartojantis įrenginio įrašas portale
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790165"
---
# <a name="duplicate-device-record-in-the-portal"></a>Pasikartojantis įrenginio įrašas portale

Galite matyti 2 įrenginio įrašus portale, jei įrenginys netinkamai praneša apie bendro valdymo būseną į Konfigūracijos tvarkyklės svetainę. Norėdami patikrinti įrenginio bendro valdymo būseną, peržiūrėkite **bendrai valdomo įrenginio** stulpelį Konfigūracijos tvarkyklės konsolėje. Jei stulpelis nerodomas, galite jį įtraukti dešiniuoju pelės klavišu spustelėdami bet kurią stulpelio antraštę ir pažymėdami jį sąraše.

Bendrai valdoma reikšmė turi būti **Taip**. Jei reikšmė yra **Ne**, atidarykite Konfigūracijos tvarkyklės kliento programą kliento įrenginyje ir skirtuke Bendra pažymėkite ypatybę **Bendras valdymas**.

- Jei reikšmė **Įgalinta**, tai reiškia problemas su kliento ir valdymo taško ryšiu. Peržiūrėkite **CcmMessaging.log** įrenginyje, kad ištirtumėte galimas ryšio triktis.

- Jei reikšmė **Išjungta** ir įrenginys užregistruotas „Intune“, įsitikinkite, kad įrenginys gavo bendro valdymo strategiją peržiūrę **CoManagementHandler. log** įrenginyje.
