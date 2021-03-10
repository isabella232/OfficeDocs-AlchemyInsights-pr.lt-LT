---
title: "\"Windows 10\" įrenginių \"Windows 10\" įrenginių trikčių šalinimas nuotoliniu būdu su \"Microsoft Defender\" patobulinta apsauga nuo grėsmių"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693651"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="a2a10-102">"Windows 10" įrenginių "Windows 10" įrenginių trikčių šalinimas nuotoliniu būdu su "Microsoft Defender" patobulinta apsauga nuo grėsmių</span><span class="sxs-lookup"><span data-stu-id="a2a10-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="a2a10-103">Jei galite pasiekti nuotolinį kompiuterį, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a2a10-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="a2a10-104">Atsisiųskite [kliento ryšio analizatoriaus](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostikos įrankį.</span><span class="sxs-lookup"><span data-stu-id="a2a10-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="a2a10-105">Išskleiskite ir paleiskite MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="a2a10-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="a2a10-106">Raskite diagnostikos pranešimą "MDATPClientAnalyzerResult" aplanke, kuris yra tas pats aplankas, kuriame buvo atsisiųstas analizatoriaus įrankis.</span><span class="sxs-lookup"><span data-stu-id="a2a10-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="a2a10-107">Jei norite sužinoti apie ryšio arba tarpinio serverio parametrų problemas, peržiūrėkite MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="a2a10-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="a2a10-108">Norėdami sužinoti daugiau, peržiūrėkite [problemas, susijusias su parengimo mašinomis](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="a2a10-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
