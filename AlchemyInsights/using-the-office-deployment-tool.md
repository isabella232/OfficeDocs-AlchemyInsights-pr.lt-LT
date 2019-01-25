---
title: Naudodami Office diegimo įrankis
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480357"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="11f7f-102">Naudodami Office diegimo įrankis (ODT)</span><span class="sxs-lookup"><span data-stu-id="11f7f-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="11f7f-p101">Diegiate "Office 365" "Office" versijos naudodami Office diegimo įrankis (ODT). Office diegimo įrankis (setup.exe) yra paleisti iš komandinės eilutės ir naudoja XML konfigūracijos failo nustatyti, kokius parametrus taikyti, kai diegiant Office.</span><span class="sxs-lookup"><span data-stu-id="11f7f-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="11f7f-105">Atsisiųsti naujausią versiją Office diegimo įrankis iš [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="11f7f-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="11f7f-p102">Naudokite [Office tinkinimo įrankį (UŠT)](https://config.office.com) pasirinkti diegimo nuostatas ir sukurkite XML konfigūracijos failo. Eksportuoti konfigūracijos failą ir įdėkite jį vietoje ant tame pačiame aplanke, kur gyvena ant "setup.exe".</span><span class="sxs-lookup"><span data-stu-id="11f7f-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="11f7f-p103">**Pastaba:** Office diegimo problemos dažniausiai atsiranda dėl į klaidingai arba malformatted konfigūracijos failus. Siekiant išvengti tokių problemų, mes rekomenduojame, kad naudojate Office tinkinimo įrankį Norėdami sukurti konfigūracijos failą. Taip pat galite importuoti esamą konfigūracijos failus į Office tinkinimo įrankį.</span><span class="sxs-lookup"><span data-stu-id="11f7f-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="11f7f-p104">Didesnių teisių komandų eilutėje, persijunkite į tą vietą, kurioje gyvena setup.exe ir paleisti Office diegimo įrankis atsisiųsti režimu ir nurodykite konfigūracijos failą išsaugoti. Šiame pavyzdyje konfigūracijos failas pavadintas Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="11f7f-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="11f7f-113">Paleisti Office diegimo įrankis, konfigūruoti režimu ir nustatyti konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="11f7f-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="11f7f-114">**Pastaba:** Šį veiksmą turite paleisti iš kliento kompiuteryje, kuriame norite įdiegti "Office" ir tame kompiuteryje turite turėti vietos administratoriaus teises.</span><span class="sxs-lookup"><span data-stu-id="11f7f-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="11f7f-p105">Norėdami sužinoti daugiau apie jūsų "Office 365 ProPlus" visuotinio diegimo scenarijai naudojant Office diegimo įrankis, ieškokite [apžvalga Office diegimo įrankis](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Daugiau informacijos apie tai, kaip naudoti Office tinkinimo įrankį, žr [apžvalga Office tinkinimo įrankį](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="11f7f-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

