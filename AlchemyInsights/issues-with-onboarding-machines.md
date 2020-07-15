---
title: Problemos su parengimo mašinos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141654"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="a858d-102">Problemos su parengimo mašinos</span><span class="sxs-lookup"><span data-stu-id="a858d-102">Issues with onboarding machines</span></span>

<span data-ttu-id="a858d-103">Jums gali kilti problemų su parengimo mašinos MDATP paslauga.</span><span class="sxs-lookup"><span data-stu-id="a858d-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="a858d-104">Jei galite pasiekti galutinio vartotojo kompiuterį, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a858d-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="a858d-105">Atsisiųskite [kliento ryšio analizatoriaus](https://aka.ms/mdatpanalyzer) diagnostikos įrankį.</span><span class="sxs-lookup"><span data-stu-id="a858d-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="a858d-106">Ekstraktas ir paleisti MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="a858d-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="a858d-107">Raskite diagnostikos žurnalo aplanke, pavadintą MDATPClientAnalyzerResult, tą patį aplanką, kuriame analyzer įrankis yra atsisiųsti.</span><span class="sxs-lookup"><span data-stu-id="a858d-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="a858d-108">Peržiūrėkite žurnalo failą MDATPClientAnalyzer.txt, kad rastumėte ryšio arba interneto tarpinio serverio parametrų problemas.</span><span class="sxs-lookup"><span data-stu-id="a858d-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>