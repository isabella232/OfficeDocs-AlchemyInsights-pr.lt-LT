---
title: Nustatyti 0x8004de40 klaida "OneDrive"
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133984"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="d028f-102">Nustatyti 0x8004de40 klaida "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="d028f-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="d028f-103">Jei gaunate klaidos 0x8004de40 naudojant "OneDrive":</span><span class="sxs-lookup"><span data-stu-id="d028f-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="d028f-104">Iš naujo paleisti dėl nukentėjusių kompiuterio, prisijungę prie savo aktyvus Directory domeno.</span><span class="sxs-lookup"><span data-stu-id="d028f-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="d028f-105">Jei iš naujo nėra išspręsti šią problemą, atsijungti ir prisijungti įrenginį iš Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d028f-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="d028f-106">**Pastaba**: turite būti įmonės tinklo atlikdami šiuos veiksmus.</span><span class="sxs-lookup"><span data-stu-id="d028f-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="d028f-107">Nereikia atlikti šiuos veiksmus, kai jūs negalite prisijungti prie savo įmonės infrastruktūrą (pavyzdžiui, kelionės metu).</span><span class="sxs-lookup"><span data-stu-id="d028f-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="d028f-108">Atidarykite didesnių teisių komandų eilutę.</span><span class="sxs-lookup"><span data-stu-id="d028f-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="d028f-109">Atidarykite komandų eilutę, spustelėkite - **pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**ir spustelėkite **paleisti kaip administratorius**.</span><span class="sxs-lookup"><span data-stu-id="d028f-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="d028f-110">Įveskite *dsregcmd /leave* ir paspauskite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="d028f-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="d028f-111">Kai baigtas, įveskite *dsregcmd /join* ir paspauskite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="d028f-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="d028f-112">Kai baigtas, uždaryti į komandų eilutę.</span><span class="sxs-lookup"><span data-stu-id="d028f-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="d028f-113">Iš naujo paleiskite kompiuterį ir prisijunkite prie "OneDrive".</span><span class="sxs-lookup"><span data-stu-id="d028f-113">Reboot the computer, and log into OneDrive.</span></span>