---
title: Klausimai apie tai, kaip naudoti Office diegimo įrankis (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925352"
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
  

