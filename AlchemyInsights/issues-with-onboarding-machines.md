---
title: Problemos, susijusios su parengimo naudoti įrenginius su „Microsoft“ sargyba pabaigos taškams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901575"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="d3f1d-102">Problemos, susijusios su parengimo naudoti įrenginius su „Microsoft“ sargyba pabaigos taškams</span><span class="sxs-lookup"><span data-stu-id="d3f1d-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="d3f1d-103">Gali kilti problemų dėl parengimo naudoti įrenginius MDE tarnybose.</span><span class="sxs-lookup"><span data-stu-id="d3f1d-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="d3f1d-104">Jei galite pasiekti galutinio vartotojo įrenginį, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="d3f1d-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="d3f1d-105">Atsisiųskite naujausią [MDE kliento analizatoriaus](https://aka.ms/betamdeanalyzer) diagnostikos įrankio peržiūros versiją.</span><span class="sxs-lookup"><span data-stu-id="d3f1d-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="d3f1d-106">Dešiniuoju pelės mygtuku spustelėkite **MDEClientAnalyzer.cmd** ir pasirinkite „Paleisti kaip administratorių“.</span><span class="sxs-lookup"><span data-stu-id="d3f1d-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="d3f1d-107">Vykdykite visur nurodymus, pateiktus **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="d3f1d-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="d3f1d-108">Norėdami matyti daugiau daugiažodžių žurnalų, peržiūrėkite sukurtą pakatalogį, pavadinimu **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="d3f1d-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="d3f1d-109">Jei reikia papildomų nurodymų, susisiekite su [„Microsoft“ pabaigos taško sargybos palaikymo tarnyba](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) ir pateikite gautą MDEClientAnalyzerResult.zip failą analizei.</span><span class="sxs-lookup"><span data-stu-id="d3f1d-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
