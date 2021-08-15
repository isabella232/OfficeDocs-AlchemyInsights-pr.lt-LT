---
title: Neveikia atidarymas naudojant "Explorer"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011344"
---
# <a name="open-with-explorer-isnt-working"></a>Neveikia atidarymas naudojant "Explorer"

Jei **parinktis Atidaryti naudojant "Explorer"** **arba** Rodinys failų naršyklėje neveikia, įsitikinkite, kad "WebClient" tarnyba **nustatyta** kaip Veikia, atlikite toliau nurodytus veiksmus. Pvz., gali užtrukti ilgai atidaryti SharePoint arba "OneDrive", kai tarnyba neveikia. 
  
1. Ieškos Windows įveskite Vykdyti, pasirinkite vykdyti kompiuterio taikomąją programą, įveskite services.msc, tada pasirinkite **Enter**.
    
2. Slinkite žemyn iki "WebClient" tarnybos ir patikrinkite **stulpelį** Būsena. Jei "WebClient" tarnybos būsena **neveikia**, dukart spustelėkite tarnybą, spustelėkite **Pradėti**, tada spustelėkite **Gerai**. Jei reikia, įgalinkite tarnybą  lauke Paleisties tipas **pasirinkdami** Neautomatinis **arba** Automatinis. 
    
> [!NOTE]
> Norėdami šalinti failų naršyklės atidarymo triktis, žr. [Atidaryti naudojant "Explorer".](https://go.microsoft.com/fwlink/?linkid=871665) Naršykite sinchronizavimą kaip geresnę alternatyvą: [SharePoint failus su naujuoju "OneDrive" sinchronizavimo programa klientu.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

