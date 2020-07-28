---
title: Intune įrenginių inventorius
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439658"
---
# <a name="intune-device-inventory"></a>Intune įrenginių inventorius

Įrenginių ašmenys suteikia administratoriui įžvalgą apie įrenginius, kurie yra valdomi "Intune", kiekvienam įrenginiui. Rodoma informacija apima: aparatūrą, aptiktas programas, įrenginio atitikties būseną ir įrenginio konfigūracijos būseną.

Atsargų duomenys aparatinei įrangai ir aptiktosioms programoms renkami septynių dienų ciklu. Nurodytos taikomosios programos ir konkretūs aparatūros elementai skiriasi priklausomai nuo įrenginio operacinės sistemos ir nuo to, ar įrenginys yra asmeniškai, ar priklausantis įmonei.

Daugiau informacijos [ieškokite įrenginio informacijoje in Intune](https://docs.microsoft.com/intune/device-inventory).

**DUK**

Klausimas: Aš negaunu visą inventoriaus sąrašą programų, esančių Intune-enrolled Windows prietaisai. kodėlgi ne?

A: Šiuo metu išvardytos tik šiuolaikinės programėlės, skirtos "Windows 10" kompiuteriams, kurie identifikuojami kaip įmonės įrenginiai. "Intune" nerenka informacijos apie šiuose įrenginiuose įdiegtas "Win32" programas.

Kl.: Kodėl telefono numeriai renkami ne iš visų įrenginių?

A: Telefonai, priskiriami įmonės įrenginiams intune, neidentifikuojami su visu telefono numeriu, kai, pvz., paleidžiate mobiliojo įrenginio atsargų ataskaitą. Bring-you-own-device telefono numeriai visada iš dalies užmaskuotas žvaigždutėmis (****), ir rodo tik paskutinius keturis skaitmenis.