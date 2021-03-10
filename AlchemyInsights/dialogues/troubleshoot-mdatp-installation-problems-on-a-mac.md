---
title: MDATP diegimo problemų šalinimas "Mac" kompiuteryje
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696102"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="5c698-102">MDATP diegimo problemų šalinimas "Mac" kompiuteryje</span><span class="sxs-lookup"><span data-stu-id="5c698-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="5c698-103">Nepavykus įdiegti neautomatiškai, diegimo vediklio **suvestinės** puslapyje rodomas šis klaidos pranešimas:</span><span class="sxs-lookup"><span data-stu-id="5c698-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="5c698-104">"Diegiant įvyko klaida.</span><span class="sxs-lookup"><span data-stu-id="5c698-104">"An error occurred during installation.</span></span> <span data-ttu-id="5c698-105">Diegimo programa aptiko klaidą, dėl kurios nepavyko įdiegti.</span><span class="sxs-lookup"><span data-stu-id="5c698-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="5c698-106">Kreipkitės pagalbos į programinės įrangos gamintoją. "</span><span class="sxs-lookup"><span data-stu-id="5c698-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="5c698-107">Naudojant MDM įdiegtį, puslapyje rodomas bendrasis diegimo gedimas.</span><span class="sxs-lookup"><span data-stu-id="5c698-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="5c698-108">Nors mes negalime Rodyti tikslių klaidų galutiniams vartotojams, mes saugome žurnalo failą su diegimo eiga, aplanke **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="5c698-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="5c698-109">Kiekvienas diegimo seansas prideda prie šio žurnalų failo.</span><span class="sxs-lookup"><span data-stu-id="5c698-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="5c698-110">Norėdami išvesti tik paskutinį diegimo seansą, naudokite `sed` .</span><span class="sxs-lookup"><span data-stu-id="5c698-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="5c698-111">Jei norite sužinoti daugiau, peržiūrėkite ["Microsoft Defender ATP for Mac" diegimo problemų diagnostiką](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="5c698-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
