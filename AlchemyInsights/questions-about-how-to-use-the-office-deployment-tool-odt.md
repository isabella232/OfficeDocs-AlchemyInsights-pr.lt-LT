---
title: Klausimai, kaip naudoti "Office" diegimo įrankį (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086164"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai, kaip naudoti "Office" diegimo įrankį (ODT)

Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Atsisiuntę failą, vykdykite išskleidimą turintį vykdomąjį failą, kuriame yra "Office" diegimo įrankio vykdomoji (setupodt.exe) ir pavyzdžio konfigūracijos failas (configuration.xml).
  
 **Jei norite neįtraukti arba pašalinti "Microsoft 365" taikomąsias programas, skirtas įmonės produktams iš kliento kompiuterio:**
  
Diegiant "Microsoft 365" taikomąsias programas įmonėms, galite išskirti konkrečius produktus. Norėdami tai padaryti, atlikite veiksmus, skirtus įdiegti "Office" su ODT, tačiau į konfigūracijos failą įtraukite ExcludeApp elementą. Pvz., šis konfigūracijos failas įdiegia visas "Microsoft" 365 taikomąsias programas, skirtas "Enterprise" produktams, išskyrus "Publisher":
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

["Office" diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

