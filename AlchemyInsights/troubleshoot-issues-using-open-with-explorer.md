---
title: Trikčių šalinimas naudojant "Open with Explorer"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759700"
---
# <a name="fix-problems-with-open-with-explorer"></a>"Open with Explorer" problemų sprendimas

Dažniausiai pasitaikančios problemos, susijusios su dokumentų bibliotekos atidaryme "SharePoint" arba "OneDrive", sprendimas naudojant komandą **Atidaryti naudojant "Explorer":** 
  
- Naudokite "Internet Explorer 10" arba "Internet Explorer 11". **Atidaryti naudojant "Explorer"** nesuderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kitais. **Atidaryti naudojant "Internet Explorer"** išjungta visose naršyklėse, išskyrus "Internet Explorer". 
    
- **Atidaryti naudojant "Explorer"** negalima šiuolaikinėje "SharePoint" bibliotekų naudojimo patirties. Vietoj to naudokite **rodinį failų naršyklėje.** **Failų naršyklėje**pasirinkite Peržiūrėti **parinktis** \> Rodinys . "File Explorer" peržiūra nesuderinama su "Microsoft Edge", "Google Chrome", "Firefox" ir kt. **Failų naršyklėje galima** tik programoje "Internet Explorer". 
    
- Įsitikinkite, kad WebClient tarnyba veikia. "Windows" ieškos lauke įveskite vykdyti, pasirinkite programėlę Vykdyti darbalaukį, įveskite services.msc, tada paspauskite Enter. Slinkite žemyn iki WebClient tarnybos ir įsitikinkite, kad stulpelyje **Būsena** rodoma "Vykdoma". Jei taip nėra, dukart spustelėkite tarnybą, spustelėkite **Pradėti**, tada spustelėkite **Gerai**. (Pirmiausia gali tekti įjungti tarnybą lauke **Paleisties tipas** pasirinkdami **Rankinis** arba **Automatinis.)** 
    
> [!NOTE]
> Bibliotekos atidarymas failų naršyklėje yra patogus, jei reikia kopijuoti arba perkelti kelis failus ir aplankus vieną kartą, bet jei norite reguliariai dirbti bibliotekoje, rekomenduojame ją sinchronizuoti. Norėdami šalinti failų naršyklės atidarymo triktis, [žr.](https://go.microsoft.com/fwlink/?linkid=871665) Informacijos apie sinchronizavimo nustatymą [ieškokite "SharePoint" failų sinchronizavimas su nauju "OneDrive" sinchronizavimo klientu](https://go.microsoft.com/fwlink/?linkid=871666).
  
Daugiau informacijos rasite straipsnyje [Kaip naudoti komandą "Atidaryti naudojant "Explorer", kad būtų išspręstos "SharePoint Online" trikčių diagnostikos priemonės.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

