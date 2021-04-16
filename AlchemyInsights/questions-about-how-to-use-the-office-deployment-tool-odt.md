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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="3c314-102">Klausimai apie tai, kaip naudoti "Office" diegimo įrankį (ODT)</span><span class="sxs-lookup"><span data-stu-id="3c314-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="3c314-103">Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="3c314-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="3c314-104">Atsisiuntę failą, paleiskite savaime išskleidžiantį vykdomąjį failą, kuriame yra "Office" diegimo įrankio vykdomasis (setup.exe) ir konfigūracijos failo pavyzdys (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="3c314-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="3c314-105">**Norėdami pašalinti arba pašalinti "Microsoft 365" programėles, skirtas įmonės produktams, iš klientų kompiuterių:**</span><span class="sxs-lookup"><span data-stu-id="3c314-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="3c314-106">Diegdami "Microsoft 365" taikomąsias programas įmonėms, galite neįtraukti konkrečių produktų.</span><span class="sxs-lookup"><span data-stu-id="3c314-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="3c314-107">Norėdami tai padaryti, atlikite "Office" diegimo su ODT veiksmus, bet įtraukite "ExcludeApp" elementą į konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="3c314-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="3c314-108">Pvz., šis konfigūracijos failas įdiegia visas "Microsoft 365" taikomąsias programas, skirtas įmonės produktams, išskyrus "Publisher":</span><span class="sxs-lookup"><span data-stu-id="3c314-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="3c314-109">"Office" diegimo įrankio apžvalga</span><span class="sxs-lookup"><span data-stu-id="3c314-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

