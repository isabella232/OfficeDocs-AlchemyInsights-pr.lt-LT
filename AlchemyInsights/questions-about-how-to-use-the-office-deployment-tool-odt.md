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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="b6f73-102">Klausimai apie tai, kaip naudoti "Office" diegimo įrankį (ODT)</span><span class="sxs-lookup"><span data-stu-id="b6f73-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="b6f73-103">Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="b6f73-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="b6f73-104">Atsisiuntę failą, paleiskite savaime išsiskleidžiančią vykdomąjį failą, kuriame yra "Office" visuotinio diegimo įrankis vykdomąjį failą (setup.exe) ir konfigūracijos failo pavyzdys (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="b6f73-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="b6f73-105">**Norėdami išskirti arba pašalinti "Microsoft 365" programėlių įmonės produktams iš kliento kompiuterių:**</span><span class="sxs-lookup"><span data-stu-id="b6f73-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="b6f73-106">Diegdami "Microsoft 365" programėles įmonėms, galite neįtraukti konkrečių produktų.</span><span class="sxs-lookup"><span data-stu-id="b6f73-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="b6f73-107">Norėdami tai padaryti, atlikite "Office" diegimo su ODT veiksmus, bet įtraukite elementą ExcludeApp į konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="b6f73-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="b6f73-108">Pavyzdžiui, šis konfigūracijos failas įdiegia visas "Microsoft 365" programėles, skirtas įmonės produktams, išskyrus "Publisher":</span><span class="sxs-lookup"><span data-stu-id="b6f73-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="b6f73-109">"Office" diegimo įrankio apžvalga</span><span class="sxs-lookup"><span data-stu-id="b6f73-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

