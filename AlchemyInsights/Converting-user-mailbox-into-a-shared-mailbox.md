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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496443"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Konvertuoti į bendrai naudojamos pašto dėžutės vartotojo pašto dėžutė

Tik galite konvertuoti vartotojo pašto dėžutės bendrinamos pašto dėžutės jei vartotojas turi keistis licenciją. Konvertavus į pašto dėžutę, ji ir toliau bus rodomi į aktyvių vartotojų sąrašą, nes tame sąraše yra bendrai naudojamos pašto dėžutės. Vis dėlto konvertuoti pašto dėžutės taip pat pasirodys sąraše bendrai naudojamos pašto dėžutės. 
  
Jei bandysite konvertuoti pašto dėžutės Exchange administratoriaus konsolėje ir konvertavimo nepavyksta, išvalykite naršyklės talpyklą ir slapukus, ir bandykite dar kartą. Jei vis tiek neveikia, bandykite konvertuoti pašto dėžutės Exchange valdymo aplinkoje vykdydami šią komandą:
  
```
Set-Mailbox -Type Shared
```

Daugiau pašto dėžučių konvertavimas informacija pateikiama [konvertuoti bendrinamos pašto dėžutės vartotojo pašto dėžutės](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
