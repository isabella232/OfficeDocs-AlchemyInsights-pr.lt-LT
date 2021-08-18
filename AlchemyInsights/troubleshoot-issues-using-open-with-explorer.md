---
title: Trikčių šalinimas naudojant "Open with Explorer"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323574"
---
# <a name="fix-problems-with-open-with-explorer"></a>Problemų, susijusių su atidarymu naudojant "Explorer", sprendimas

Dažniausiai pasitaikančių problemų, susijusių su dokumentų bibliotekos atidarymu SharePoint arba "OneDrive" naudojant komandą **Atidaryti naudojant "Explorer":** 
  
- Naudokite Internet Explorer 10 "Internet Explorer 11". **Atidaryti naudojant "Explorer"** nesuderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kitais. **Atidaryti naudojant "Explorer"** išjungta visose naršyklėse, išskyrus "Internet Explorer". 
    
- **Atidaryti naudojant "Explorer"** negalima naudojant šiuolaikinę "SharePoint bibliotekų patirtį. Naudokite **Rodinį failų naršyklėje.** Pasirinkite **Rodinio parinktys Rodinys** failų \> **naršyklėje**. Rodinys failų naršyklėje nesuderinamas su "Microsoft Edge", "Google Chrome", "Firefox" ir kitais. **Peržiūrėkite failų naršyklėje** tik "Internet Explorer". 
    
- Įsitikinkite, kad veikia "WebClient" tarnyba. Ieškos Windows įveskite vykdyti, pasirinkite vykdyti kompiuterio taikomąją programą, įveskite services.msc, tada paspauskite "Enter". Slinkite žemyn iki "WebClient" tarnybos ir įsitikinkite, **kad stulpelyje** Būsena rodoma "Veikia". Jei ne, dukart spustelėkite tarnybą, spustelėkite **Pradėti**, tada spustelėkite **Gerai**. (Pirmiausia gali tekti įgalinti tarnybą lauke  Paleisties tipas pasirinkus Neautomatinis  **arba** Automatinis.) 
    
**Pastaba:** bibliotekos atidarymas failų naršyklėje yra patogus, jei reikia kopijuoti arba perkelti kelis failus ir aplankus vieną kartą, bet jei norite reguliariai dirbti bibliotekoje, rekomenduojame ją sinchronizuoti. Norėdami šalinti failų naršyklės atidarymo triktis, žr. [Atidaryti naudojant "Explorer".](https://go.microsoft.com/fwlink/?linkid=871665) Informacijos apie sinchronizavimo nustatymą žr. [Failų sinchronizavimas SharePoint su naujuoju "OneDrive" sinchronizavimo programa klientu](https://go.microsoft.com/fwlink/?linkid=871666).
  
Daugiau informacijos [žr. straipsnyje Kaip naudoti komandą "Atidaryti naudojant "Explorer",](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) kad būtų SharePoint internete. 
  

