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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774899"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai, kaip naudoti "Office" diegimo įrankį (ODT)

Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Atsisiuntę failą, vykdykite išskleidimą turintį vykdomąjį failą, kuriame yra "Office" diegimo įrankio vykdomoji (setup.exe) ir pavyzdžio konfigūracijos failas (configuration.xml).
  
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
  

