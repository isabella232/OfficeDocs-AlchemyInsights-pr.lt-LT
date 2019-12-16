---
title: "\"OneDrive\" klaidos ištaisymas 0x8004de40"
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052045"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="14a55-102">"OneDrive" klaidos ištaisymas 0x8004de40</span><span class="sxs-lookup"><span data-stu-id="14a55-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="14a55-103">Jei įvyksta klaida 0x8004de40 su "OneDrive":</span><span class="sxs-lookup"><span data-stu-id="14a55-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="14a55-104">Perkraukite pažeistą kompiuterį, o prijungtas prie jūsų Acitve katalogo domenas.</span><span class="sxs-lookup"><span data-stu-id="14a55-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="14a55-105">Jei iš naujo nepavyksta išspręsti problemos, atsijungti ir prisijungti savo įrenginį iš Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14a55-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="14a55-106">**Pastaba**: atlikdami šiuos veiksmus, turėtumėte būti įmonės tinkle.</span><span class="sxs-lookup"><span data-stu-id="14a55-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="14a55-107">Neatlikite šių veiksmų, kai negalite prisijungti prie įmonės infrastruktūros (pvz., keliaudami).</span><span class="sxs-lookup"><span data-stu-id="14a55-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="14a55-108">Atidarykite didesnių teisių komandų eilutę.</span><span class="sxs-lookup"><span data-stu-id="14a55-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="14a55-109">Norėdami atidaryti didesnių teisių komandų eilutę, spustelėkite **pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**, tada spustelėkite **paleisti administratoriaus teisėmis**.</span><span class="sxs-lookup"><span data-stu-id="14a55-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="14a55-110">Tipo *dsregcmd/atostogos* ir paspauskite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="14a55-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="14a55-111">Baigę įveskite *dsregcmd/Join* ir paspauskite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="14a55-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="14a55-112">Baigę uždarykite komandinę eilutę.</span><span class="sxs-lookup"><span data-stu-id="14a55-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="14a55-113">Perkraukite kompiuterį ir prisijunkite prie OneDrive.</span><span class="sxs-lookup"><span data-stu-id="14a55-113">Reboot the computer, and log into OneDrive.</span></span>