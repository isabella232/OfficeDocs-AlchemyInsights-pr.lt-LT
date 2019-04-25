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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371776"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="136b5-102">Klausimai apie tai, kaip naudoti Office diegimo įrankis (ODT)</span><span class="sxs-lookup"><span data-stu-id="136b5-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="136b5-103">Atsisiųskite Office diegimo įrankis iš [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="136b5-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="136b5-104">Po atsisiųsti failą, paleiskite savaime išsiskleidžiantis vykdomasis failas, kuriame yra Office diegimo įrankis vykdomąjį (setup.exe) ir imties konfigūracijos failas (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="136b5-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="136b5-105">**Norėdami pašalinti arba pašalinti "Office 365 ProPlus" produktus iš kliento kompiuteryje:**</span><span class="sxs-lookup"><span data-stu-id="136b5-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="136b5-106">Diegiant "Office 365 ProPlus", galite pašalinti konkrečius produktus.</span><span class="sxs-lookup"><span data-stu-id="136b5-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="136b5-107">Norėdami tai padaryti, atlikite nurodytus veiksmus, skirtus įdiegti Office, ODT, bet ExcludeApp elementu jūsų konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="136b5-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="136b5-108">Pvz., šis konfigūracijos failas įdiegia visus "Office 365 ProPlus" produktai, išskyrus leidėjas:</span><span class="sxs-lookup"><span data-stu-id="136b5-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="136b5-109">Office diegimo įrankis apžvalga</span><span class="sxs-lookup"><span data-stu-id="136b5-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

