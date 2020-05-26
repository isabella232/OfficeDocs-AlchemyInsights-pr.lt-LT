---
title: 618 Kalendoriaus bendrinimo strategija
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373007"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="8c38c-102">Strategijos klaida bendrinant kalendorių</span><span class="sxs-lookup"><span data-stu-id="8c38c-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="8c38c-103">Atlikite vieną iš šių veiksmų, atsižvelgdami į savo situaciją:</span><span class="sxs-lookup"><span data-stu-id="8c38c-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="8c38c-104">Prisijunkite prie "Exchange Online" naudodami nuotolinę "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="8c38c-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="8c38c-105">Daugiau informacijos [ieškokite Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8c38c-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="8c38c-106">Vietiniame serveryje atidarykite "Exchange" valdymo aplinką.</span><span class="sxs-lookup"><span data-stu-id="8c38c-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="8c38c-107">Nustatykite vartotojui priskirtą bendrinimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="8c38c-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="8c38c-108">Norėdami tai padaryti, vykdykite šią komandą ir atkreipkite dėmesį, kad strategija grįžo:</span><span class="sxs-lookup"><span data-stu-id="8c38c-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="8c38c-109">Atnaujinkite vartotojo bendrinimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="8c38c-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="8c38c-110">Jei norite tai padaryti, atlikite tokius veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8c38c-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="8c38c-111">Atidarykite "Exchange" administravimo centrą.</span><span class="sxs-lookup"><span data-stu-id="8c38c-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="8c38c-112">Spustelėkite **Organizacija**, tada dukart spustelėkite strategiją, priskirtą vartotojui dalyje **Individualus bendrinimas**.</span><span class="sxs-lookup"><span data-stu-id="8c38c-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="8c38c-113">Tai politika, kuri buvo grąžinta 2 veiksme.</span><span class="sxs-lookup"><span data-stu-id="8c38c-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="8c38c-114">Puslapyje Bendrinimo taisyklė pasirinkite kalendoriaus bendrinimo lygį, kurį norite leisti dalyje **Nurodykite, kokią informaciją norite bendrinti;** spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="8c38c-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="8c38c-115">Daugiau informacijos rasite: ["Strategija neleidžia suteikti teises šiame lygyje vienam ar daugiau gavėjo (-ų)" klaida, kai vartotojas bando bendrinti kalendorių](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="8c38c-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
