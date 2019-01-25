---
title: Konvertuoti vartotojo pašto dėžutės į bendrinamą pašto dėžutę?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480348"
---
Tik galite konvertuoti vartotojo pašto dėžutės bendrinamos pašto dėžutės jei vartotojas turi keistis licenciją. Konvertavus į pašto dėžutę, ji ir toliau bus rodomi į aktyvių vartotojų sąrašą, nes tame sąraše yra bendrai naudojamos pašto dėžutės. Vis dėlto konvertuoti pašto dėžutės taip pat pasirodys sąraše bendrai naudojamos pašto dėžutės. 
  
Jei bandysite konvertuoti pašto dėžutės Exchange administratoriaus konsolėje ir konvertavimo nepavyksta, išvalykite naršyklės talpyklą ir slapukus, ir bandykite dar kartą. Jei vis tiek neveikia, bandykite konvertuoti pašto dėžutės Exchange valdymo aplinkoje vykdydami šią komandą:
  
```
Set-Mailbox -Type Shared
```

Daugiau pašto dėžučių konvertavimas informacija pateikiama [konvertuoti bendrinamos pašto dėžutės vartotojo pašto dėžutės](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
