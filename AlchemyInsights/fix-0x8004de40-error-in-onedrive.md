---
title: Klaidos 0x8004de40 taisymas "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716036"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="5c2f0-102">Klaidos 0x8004de40 taisymas "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="5c2f0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="5c2f0-103">Jei su "OneDrive" gaunate klaidos pranešimą 0x8004de40:</span><span class="sxs-lookup"><span data-stu-id="5c2f0-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="5c2f0-104">Perkraukite paveiktą kompiuterį, kai prijungtas prie acitve katalogo domeno.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="5c2f0-105">Jei iš naujo neišsprendžia problemos, atjunkite ir vėl prisijunkite prie įrenginio iš "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="5c2f0-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="5c2f0-106">**Pastaba:** atlikdami šiuos veiksmus turėtumėte būti įmonės tinkle.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="5c2f0-107">Neatlikite šių veiksmų, kai negalite prisijungti prie įmonės infrastruktūros (pvz., keliaudami).</span><span class="sxs-lookup"><span data-stu-id="5c2f0-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="5c2f0-108">Atidarykite didesnių teisių komandinę eilutę.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="5c2f0-109">Norėdami atidaryti didesnių teisių komandų eilutę, spustelėkite - **Pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**, tada spustelėkite **Paleisti administratoriaus teisėmis**.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="5c2f0-110">Įveskite *dsregcmd /leave* ir paspauskite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="5c2f0-111">Baigę įveskite *dsregcmd /join* ir paspauskite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="5c2f0-112">Baigę uždarykite komandinę eilutę.</span><span class="sxs-lookup"><span data-stu-id="5c2f0-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="5c2f0-113">Perkraukite kompiuterį ir prisijunkite prie "OneDrive".</span><span class="sxs-lookup"><span data-stu-id="5c2f0-113">Reboot the computer, and log into OneDrive.</span></span>