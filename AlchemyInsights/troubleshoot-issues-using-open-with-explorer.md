---
title: Trikčių šalinimas naudojant "Explorer"
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659066"
---
# <a name="fix-problems-with-open-with-explorer"></a>Su naršykle atidarytų problemų sprendimas

Išspręskite įprastas problemas, susijusias su "SharePoint" arba "OneDrive" dokumentų bibliotekos atidarymu naudodami komandą **Atidaryti naudojant Explorer** : 
  
- Naudokite "Internet Explorer 10" arba "Internet Explorer 11". **Atidaryti naudojant "Explorer** " nesuderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kt. **Atidaryti naudojant "Explorer"** išjungta visose naršyklėse, išskyrus "Internet Explorer". 
    
- **Atidaryti naudojant "Explorer"** negalima šiuolaikinėje "SharePoint" bibliotekų srityje. Vietoj to naudokite **rodinį failų naršyklėje** . Pasirinkite **Peržiūrėti parinkčių** \> **rodinį failų naršyklėje**. Rodinys failų naršyklėje nesuderinamas su "Microsoft Edge", "Google Chrome", "Firefox" ir kitais. **Peržiūrėti failų naršyklėje** galima tik naudojant "Internet Explorer". 
    
- Įsitikinkite, kad veikia WebClient tarnyba. "Windows" ieškos lauke įveskite vykdyti, pasirinkite paleisti kompiuterio taikomąją programą, įveskite Services. msc, tada paspauskite klavišą "įvesti". Slinkite žemyn iki "WebClient" tarnybos ir įsitikinkite, kad stulpelyje **Būsena** rodoma "veikia". Jei ne, dukart spustelėkite tarnybą, spustelėkite **pradėti**, tada spustelėkite **gerai**. (Pirmiausia gali reikėti įgalinti paslaugą, lauke **Paleisties tipas** pasirinkę **Rankinis** arba **Automatinis** .) 
    
> [!NOTE]
> Jei norite, kad būtų galima kopijuoti arba perkelti kelis failus ir aplankus, galite atidaryti biblioteką failų naršyklėje, bet jei norite reguliariai dirbti bibliotekoje, rekomenduojame ją sinchronizuoti. Norėdami šalinti problemas, atidaromas failų naršyklėje, žiūrėkite [Atidaryti naudojant "Explorer"](https://go.microsoft.com/fwlink/?linkid=871665). Informacijos apie sinchronizavimo nustatymą ieškokite ["SharePoint" failų sinchronizavimas naudojant naująjį "OneDrive" sinchronizavimo klientą](https://go.microsoft.com/fwlink/?linkid=871666).
  
Daugiau informacijos rasite straipsnyje [kaip naudoti komandą Atidaryti naudojant "Explorer", kad išspręstumėte "SharePoint Online" problemas](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

