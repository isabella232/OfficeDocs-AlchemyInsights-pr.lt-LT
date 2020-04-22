---
title: Atidaryti naudojant "Explorer" neveikia
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713042"
---
# <a name="open-with-explorer-isnt-working"></a>Atidaryti naudojant "Explorer" neveikia

Jei **atidaryti naudojant "Explorer"** arba **peržiūrėti failų naršyklėje** neveikia įsitikinkite, kad WebClient tarnyba nustatyta **kaip veikia** atlikdami toliau nurodytus veiksmus. Pavyzdžiui, gali ilgai užtrukti atidaryti "SharePoint" arba "OneDrive" biblioteką, kai tarnyba neveikia. 
  
1. "Windows" ieškos lauke įveskite vykdyti, pasirinkite programėlę Paleisti darbalaukį, įveskite services.msc, tada pasirinkite **Enter**.
    
2. Slinkite žemyn iki WebClient tarnybos ir patikrinkite stulpelį **Būsena.** Jei WebClient tarnybos būsena **neveikia**, dukart spustelėkite tarnybą, spustelėkite **pradėti**, ir tada spustelėkite **gerai**. Jei reikia, įjunkite tarnybą lauke **Paleisties tipas** pasirinkdami **Rankinis** arba **Automatinis.** 
    
> [!NOTE]
> Norėdami šalinti failų naršyklės atidarymo triktis, [žr.](https://go.microsoft.com/fwlink/?linkid=871665) Naršykite sinchronizavimą kaip geresnę alternatyvą: [sinchronizuokite "SharePoint" failus su nauju "OneDrive" sinchronizavimo klientu](https://go.microsoft.com/fwlink/?linkid=871666). 
  

