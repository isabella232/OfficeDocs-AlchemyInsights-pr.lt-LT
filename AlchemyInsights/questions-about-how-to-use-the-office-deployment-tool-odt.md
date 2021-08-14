---
title: Klausimai apie tai, kaip naudoti Office diegimo įrankį (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959691"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai apie tai, kaip naudoti Office diegimo įrankį (ODT)

Atsisiųskite Office diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Atsisiuntę failą paleiskite savaime išskleidžiantį vykdomąjį failą, kuriame yra "Office" diegimo įrankio vykdomasis ("setup.exe") ir konfigūracijos failo pavyzdys (configuration.xml).
  
 **Norėdami pašalinti arba pašalinti "Microsoft 365" programos įmonėms produktus iš kliento kompiuterių:**
  
Diegdami "Microsoft 365" programos įmonėms, galite neįtraukti konkrečių produktų. Norėdami tai padaryti, atlikite veiksmus, Office odt, bet įtraukite "ExcludeApp" elementą į konfigūracijos failą. Pvz., šis konfigūracijos failas įdiegia visus "Microsoft 365" programos įmonėms, išskyrus Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

["Office" diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

