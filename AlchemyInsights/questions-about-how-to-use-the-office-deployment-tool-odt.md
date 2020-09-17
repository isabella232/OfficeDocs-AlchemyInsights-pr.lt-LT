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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="12fcf-102">Klausimai, kaip naudoti "Office" diegimo įrankį (ODT)</span><span class="sxs-lookup"><span data-stu-id="12fcf-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="12fcf-103">Atsisiųskite "Office" diegimo įrankį iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="12fcf-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="12fcf-104">Atsisiuntę failą, vykdykite išskleidimą turintį vykdomąjį failą, kuriame yra "Office" diegimo įrankio vykdomoji (setup.exe) ir pavyzdžio konfigūracijos failas (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="12fcf-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="12fcf-105">**Jei norite neįtraukti arba pašalinti "Microsoft 365" taikomąsias programas, skirtas įmonės produktams iš kliento kompiuterio:**</span><span class="sxs-lookup"><span data-stu-id="12fcf-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="12fcf-106">Diegiant "Microsoft 365" taikomąsias programas įmonėms, galite išskirti konkrečius produktus.</span><span class="sxs-lookup"><span data-stu-id="12fcf-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="12fcf-107">Norėdami tai padaryti, atlikite veiksmus, skirtus įdiegti "Office" su ODT, tačiau į konfigūracijos failą įtraukite ExcludeApp elementą.</span><span class="sxs-lookup"><span data-stu-id="12fcf-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="12fcf-108">Pvz., šis konfigūracijos failas įdiegia visas "Microsoft" 365 taikomąsias programas, skirtas "Enterprise" produktams, išskyrus "Publisher":</span><span class="sxs-lookup"><span data-stu-id="12fcf-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="12fcf-109">"Office" diegimo įrankio apžvalga</span><span class="sxs-lookup"><span data-stu-id="12fcf-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

