---
title: Konvertuoti vartotojo pašto dėžutės į bendrinamą pašto dėžutę?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374331"
---
Tik galite konvertuoti vartotojo pašto dėžutės bendrinamos pašto dėžutės jei vartotojas turi keistis licenciją. Konvertavus į pašto dėžutę, ji ir toliau bus rodomi į aktyvių vartotojų sąrašą, nes tame sąraše yra bendrai naudojamos pašto dėžutės. Vis dėlto konvertuoti pašto dėžutės taip pat pasirodys sąraše bendrai naudojamos pašto dėžutės. 
  
Jei bandysite konvertuoti pašto dėžutės Exchange administratoriaus konsolėje ir konvertavimo nepavyksta, išvalykite naršyklės talpyklą ir slapukus, ir bandykite dar kartą. Jei vis tiek neveikia, bandykite konvertuoti pašto dėžutės Exchange valdymo aplinkoje vykdydami šią komandą:
  
```
Set-Mailbox -Type Shared
```

Daugiau pašto dėžučių konvertavimas informacija pateikiama [konvertuoti bendrinamos pašto dėžutės vartotojo pašto dėžutės](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
