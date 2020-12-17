---
title: Ką daryti, jei "Azure" funkcijos netinkamai veikia "Microsoft Edge"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583789"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="9895d-102">Ką daryti, jei "Azure" funkcijos netinkamai veikia "Microsoft Edge"</span><span class="sxs-lookup"><span data-stu-id="9895d-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="9895d-103">"Microsoft Edge" [žinomos problemos](https://go.microsoft.com/fwlink/?linkid=2140608) , kurios yra susijusios su saugos zonomis ir gali turėti įtakos, kaip "Azure" vartotojai prisijungs prie "Windows" administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="9895d-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="9895d-104">Jei kyla problemų naudojant "Azure" funkcijas su "Microsoft Edge", išbandykite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="9895d-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="9895d-105">**Pradžios** meniu ieškokite **Interneto parinktys** ir pasirinkite ją.</span><span class="sxs-lookup"><span data-stu-id="9895d-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="9895d-106">Dialogo lange **interneto ypatybės** eikite į skirtuką **Sauga** .</span><span class="sxs-lookup"><span data-stu-id="9895d-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="9895d-107">Pasirinkite **patikimų svetainių** zoną ir pasirinkite mygtuką **svetainės** .</span><span class="sxs-lookup"><span data-stu-id="9895d-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="9895d-108">Dialogo lange **patikimos svetainės** įtraukite savo šliuzo URL taip pat [https://login.microsoftonline.com](https://login.microsoftonline.com) ir [https://login.live.com](https://login.live.com) , tada pasirinkite **uždaryti**.</span><span class="sxs-lookup"><span data-stu-id="9895d-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="9895d-109">Dialogo lange **interneto ypatybės** eikite į skirtuką **Privatumas** .</span><span class="sxs-lookup"><span data-stu-id="9895d-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="9895d-110">Dalyje **iššokančių langų blokavimo programa** pasirinkite **Parametrai**.</span><span class="sxs-lookup"><span data-stu-id="9895d-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="9895d-111">Atsidariusiame dialogo lange įtraukite savo šliuzo URL, taip pat [https://login.microsoftonline.com](https://login.microsoftonline.com) ir [https://login.live.com](https://login.live.com) , tada pasirinkite **uždaryti**.</span><span class="sxs-lookup"><span data-stu-id="9895d-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>