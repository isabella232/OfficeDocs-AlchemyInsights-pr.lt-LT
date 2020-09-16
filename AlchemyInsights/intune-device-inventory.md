---
title: "\"Intune\" įrenginių inventorius"
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667886"
---
# <a name="intune-device-inventory"></a>"Intune" įrenginių inventorius

Įrenginių ašmenys suteikia administratoriui įžvalgų įrenginių dalyje valdymas, kurį naudoja "Intune" vienam įrenginiui. Rodoma informacija: aparatūra, aptiktos taikomosios programos, įrenginio atitikties būsena ir įrenginio konfigūracijos būsena.

Įrenginių atsargų duomenys ir aptiktos taikomosios programos renkamos septynių dienų ciklu. Taikomosios programos ir specifiniai aparatūros elementai skiriasi atsižvelgiant į įrenginio operacinę sistemą ir į tai, ar įrenginys yra asmeniškai, ar įmonės nuosavybė.

Daugiau informacijos rasite [įrenginio informacijos peržiūra "Intune](https://docs.microsoft.com/intune/device-inventory)".

**DUK**

K: aš negavau visos inventorizacijos programos, esančios "Intune", įtrauktų į "Windows" įrenginius. kodėlgi ne?

A: šiuo metu "Windows 10" kompiuteriuose, kurie identifikuojami kaip įmonės įrenginiai, nurodomos tik šiuolaikinės taikomosios programos. Intune nerenka informacijos apie "Win32" taikomąsias programas, įdiegtas šiuose įrenginiuose.

K: Kodėl telefono numeriai nerenkami iš visų įrenginių?

A: kai, pvz., paleidus mobiliųjų įrenginių atsargų ataskaitą, į "Intune" priskiriami telefonai, kurie priskiriami įmonės įrenginiams. "Bring-Your-Own" įrenginio telefono numeriai visada yra dalinai užmaskuoti žvaigždute (* * * *) ir rodomi tik keturi paskutiniai skaitmenys.