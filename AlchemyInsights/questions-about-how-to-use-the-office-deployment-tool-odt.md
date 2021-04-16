---
title: Klausimai apie tai, kaip naudoti "Office" diegimo įrankį (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790340"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai apie tai, kaip naudoti "Office" diegimo įrankį (ODT)

Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Atsisiuntę failą, paleiskite savaime išskleidžiantį vykdomąjį failą, kuriame yra "Office" diegimo įrankio vykdomasis (setup.exe) ir konfigūracijos failo pavyzdys (configuration.xml).
  
 **Norėdami pašalinti arba pašalinti "Microsoft 365" programėles, skirtas įmonės produktams, iš klientų kompiuterių:**
  
Diegdami "Microsoft 365" taikomąsias programas įmonėms, galite neįtraukti konkrečių produktų. Norėdami tai padaryti, atlikite "Office" diegimo su ODT veiksmus, bet įtraukite "ExcludeApp" elementą į konfigūracijos failą. Pvz., šis konfigūracijos failas įdiegia visas "Microsoft 365" taikomąsias programas, skirtas įmonės produktams, išskyrus "Publisher":
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

["Office" diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

