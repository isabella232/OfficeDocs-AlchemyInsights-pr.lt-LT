---
title: Klaidos sprendimas 0x8004de40 "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745138"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="15da4-102">Klaidos sprendimas 0x8004de40 "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="15da4-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="15da4-103">Jei gavote 0x8004de40 klaidą su "OneDrive":</span><span class="sxs-lookup"><span data-stu-id="15da4-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="15da4-104">Iš naujo paleiskite paveiktą kompiuterį, kai esate prisijungę prie "Acitve" katalogų domeno.</span><span class="sxs-lookup"><span data-stu-id="15da4-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="15da4-105">Jei perkrovimas nepadeda išspręsti problemos, prisijunkite prie įrenginio naudodami "Azure AD" ir vėl prisijunkite prie jo.</span><span class="sxs-lookup"><span data-stu-id="15da4-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="15da4-106">**Pastaba**: turite būti įmonės tinkle atlikdami šiuos veiksmus.</span><span class="sxs-lookup"><span data-stu-id="15da4-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="15da4-107">Neatlikite šių veiksmų, kai negalėsite prisijungti prie savo įmonės infrastruktūros (pvz., keliaudami).</span><span class="sxs-lookup"><span data-stu-id="15da4-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="15da4-108">Atidarykite didesnių teisių komandinę eilutę.</span><span class="sxs-lookup"><span data-stu-id="15da4-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="15da4-109">Norėdami atidaryti didesnių teisių komandinę eilutę, spustelėkite – **pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**, tada spustelėkite **paleisti administratoriaus**teisėmis.</span><span class="sxs-lookup"><span data-stu-id="15da4-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="15da4-110">Įveskite *dsregcmd/Leave* ir paspauskite " **įvesti**".</span><span class="sxs-lookup"><span data-stu-id="15da4-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="15da4-111">Baigę įveskite *dsregcmd/Join* ir paspauskite klavišą " **įvesti**".</span><span class="sxs-lookup"><span data-stu-id="15da4-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="15da4-112">Baigę uždarykite komandinę eilutę.</span><span class="sxs-lookup"><span data-stu-id="15da4-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="15da4-113">Iš naujo paleiskite kompiuterį ir Prisiregistruokite prie "OneDrive".</span><span class="sxs-lookup"><span data-stu-id="15da4-113">Reboot the computer, and log into OneDrive.</span></span>