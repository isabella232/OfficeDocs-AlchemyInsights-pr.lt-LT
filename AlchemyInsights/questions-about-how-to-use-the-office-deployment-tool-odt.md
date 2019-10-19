---
title: Klausimai apie tai, kaip naudoti Office visuotinio diegimo įrankį (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553548"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai apie tai, kaip naudoti Office visuotinio diegimo įrankį (ODT)

Atsisiųskite "Office" visuotinio diegimo įrankį iš ["Microsoft" atsisiuntimo centro](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po atsisiųsti failą, paleisti savaime išsiskleidžiantį vykdomąjį failą, kuriame yra Office diegimo įrankis vykdomąjį (Setup. exe) ir mėginio konfigūracijos failas (Configuration. XML).
  
 **Norėdami pašalinti arba pašalinti Office 365 ProPlus produktus iš kliento kompiuteryje:**
  
Diegiant Office 365 ProPlus, galite išskirti tam tikrų produktų. Norėdami tai padaryti, atlikite veiksmus įdiegti Office su ODT, bet įtraukti ExcludeApp elementas jūsų konfigūracijos failą. Pavyzdžiui, šis konfigūracijos failas įdiegia visus Office 365 ProPlus produktus, išskyrus Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

["Office" visuotinio diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

