---
title: "\"Intune\" įrenginių atsargos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014080"
---
# <a name="intune-device-inventory"></a>"Intune" įrenginių atsargos

Įrenginių ašmenys suteikia administratoriui įžvalgų apie "Intune" valdymo įrenginius pagal kiekvieną įrenginį. Rodoma informacija: Aparatūra, Aptiktos taikomosios programos, Įrenginio atitikties būsena ir Įrenginio konfigūravimo būsena.

Aparatūros ir aptiktų taikomųjų programų atsargų duomenys renkami septynių dienų ciklu. Pateiktos taikomosios programos ir konkretūs aparatūros elementai skiriasi atsižvelgiant į įrenginio operacinę sistemą ir į tai, ar įrenginys priklauso asmeniškai, ar įmonės.

Daugiau informacijos žr. [įrenginio išsami informacija "Intune"](https://docs.microsoft.com/intune/device-inventory).

**DUK**

K: negauiu viso "Intune" užregistruotuose įrenginiuose esančių taikomųjų programų Windows sąrašo. kodėlgi ne?

A: Šiuo metu tik šiuolaikinės programėlės yra išvardytos Windows 10, kurie identifikuojami kaip įmonės įrenginiai. "Intune" nerinks informacijos apie šiuose įrenginiuose įdiegtas "Win32" programas.

K: kodėl telefono numeriai renkami ne iš visų įrenginių?

A: Telefonai, priskiriami "Intune" įmonės įrenginiams, nėra identifikuojami su visu telefono numeriu, kai, pvz., vykdote mobiliųjų įrenginių atsargų ataskaitą. Jūsų pačių įrenginio telefono numeriai visada iš dalies užmaskuojami žvaigždutėmis (****) ir rodomi tik paskutiniai keturi skaitmenys.