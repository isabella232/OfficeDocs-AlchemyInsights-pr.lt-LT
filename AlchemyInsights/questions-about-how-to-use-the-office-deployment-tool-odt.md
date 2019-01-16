---
title: Klausimai apie tai, kaip naudoti Office diegimo įrankis (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301157"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Klausimai apie tai, kaip naudoti Office diegimo įrankis (ODT)

Atsisiųskite Office diegimo įrankis iš [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po atsisiųsti failą, paleiskite savaime išsiskleidžiantis vykdomasis failas, kuriame yra Office diegimo įrankis vykdomąjį (setup.exe) ir imties konfigūracijos failas (configuration.xml).
  
 **Norėdami pašalinti arba pašalinti "Office 365 ProPlus" produktus iš kliento kompiuteryje:**
  
Diegiant "Office 365 ProPlus", galite pašalinti konkrečius produktus. Norėdami tai padaryti, atlikite nurodytus veiksmus, skirtus įdiegti Office, ODT, bet ExcludeApp elementu jūsų konfigūracijos failą. Pvz., šis konfigūracijos failas įdiegia visus "Office 365 ProPlus" produktai, išskyrus leidėjas:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office diegimo įrankis apžvalga](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

