---
title: "\"Office\" diegimo įrankio naudojimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794919"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="a2265-102">"Office" diegimo įrankio naudojimas (ODT)</span><span class="sxs-lookup"><span data-stu-id="a2265-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a2265-103">Naudokite "Office" diegimo įrankį (ODT), kad įdiegtumėte "Office 365" versijas "Office".</span><span class="sxs-lookup"><span data-stu-id="a2265-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="a2265-104">"Office" diegimo įrankis (setup.exe) paleidžiamas iš komandų eilutės ir naudoja konfigūracijos XML failą, kad nustatytų, kokie parametrai turi būti taikomi diegiant "Office".</span><span class="sxs-lookup"><span data-stu-id="a2265-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="a2265-105">Atsisiųskite naujausią "Office" diegimo įrankio versiją iš ["Microsoft" atsisiuntimo centro](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a2265-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="a2265-106">Naudokite " [Office" tinkinimo įrankį (OCT)](https://config.office.com) , kad pasirinktumėte diegimo nuostatas ir SUKURTUMĖTE konfigūracijos XML failą.</span><span class="sxs-lookup"><span data-stu-id="a2265-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="a2265-107">Eksportuokite konfigūracijos failą ir padėkite jį vietiniame tame pačiame aplanke, kuriame yra setup.exe.</span><span class="sxs-lookup"><span data-stu-id="a2265-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="a2265-108">**Pastaba:** "Office" diegimo problemos paprastai kyla dėl netinkamai sukonfigūruotų arba netinkamai suformatuotų konfigūracijos failų.</span><span class="sxs-lookup"><span data-stu-id="a2265-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="a2265-109">Norėdami išvengti tokių problemų, rekomenduojame naudoti "Office" tinkinimo įrankį kuriant konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="a2265-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="a2265-110">Esamus konfigūracijos failus taip pat galite importuoti į "Office" tinkinimo įrankį.</span><span class="sxs-lookup"><span data-stu-id="a2265-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="a2265-111">Didesnių teisių komandų eilutėje įjunkite vietą, kurioje setup.exe gyvena, ir paleiskite "Office" diegimo įrankį atsisiuntimo režimu ir nustatykite ką tik įrašytą konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="a2265-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="a2265-112">Šiame pavyzdyje konfigūracijos failas pavadintas Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="a2265-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="a2265-113">4. Paleiskite "Office" diegimo įrankį konfigūravimo režimu ir nustatykite konfigūracijos failą.</span><span class="sxs-lookup"><span data-stu-id="a2265-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="a2265-114">**Pastaba:** Šį veiksmą turite atlikti iš kliento kompiuterio, kuriame norite įdiegti "Office", ir tame kompiuteryje turite turėti vietinio administratoriaus teises.</span><span class="sxs-lookup"><span data-stu-id="a2265-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="a2265-115">Norėdami sužinoti daugiau apie "Office" diegimo įrankio naudojimą "Microsoft" 365 programoms, skirtas įmonės diegimo scenarijams, skaitykite " [Office" diegimo įrankio apžvalga](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="a2265-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="a2265-116">Daugiau informacijos, kaip naudoti "Office" tinkinimo įrankį, rasite " [Office" tinkinimo įrankio apžvalga](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="a2265-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
