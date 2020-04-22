---
title: Klausimai apie tai, kaip naudoti "Office" diegimo įrankį (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698066"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai apie tai, kaip naudoti "Office" diegimo įrankį (ODT)

Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Atsisiuntę failą, paleiskite savaime išsiskleidžiančią vykdomąjį failą, kuriame yra "Office" visuotinio diegimo įrankis vykdomąjį failą (setup.exe) ir konfigūracijos failo pavyzdys (configuration.xml).
  
 **Norėdami išskirti arba pašalinti "Microsoft 365" programėlių įmonės produktams iš kliento kompiuterių:**
  
Diegdami "Microsoft 365" programėles įmonėms, galite neįtraukti konkrečių produktų. Norėdami tai padaryti, atlikite "Office" diegimo su ODT veiksmus, bet įtraukite elementą ExcludeApp į konfigūracijos failą. Pavyzdžiui, šis konfigūracijos failas įdiegia visas "Microsoft 365" programėles, skirtas įmonės produktams, išskyrus "Publisher":
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

["Office" diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

