---
title: 618 kalendoriaus naudojimo strategija
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684238"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="0b827-102">Strategijos klaida, kai dalijamasi su kalendoriumi</span><span class="sxs-lookup"><span data-stu-id="0b827-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="0b827-103">Atsižvelgdami į situaciją atlikite vieną iš šių veiksmų:</span><span class="sxs-lookup"><span data-stu-id="0b827-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="0b827-104">Prisijungimas prie "Exchange Online" naudojant nuotolinį "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="0b827-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="0b827-105">Daugiau informacijos ieškokite [prisijungimas prie "Exchange Online" naudojant nuotolinę "PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)".</span><span class="sxs-lookup"><span data-stu-id="0b827-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="0b827-106">Vietiniame serveryje atidarykite "Exchange" valdymo aplinką.</span><span class="sxs-lookup"><span data-stu-id="0b827-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="0b827-107">Nustatykite vartotojui priskirtą bendro naudojimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="0b827-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="0b827-108">Norėdami tai padaryti, vykdykite šią komandą ir užsirašykite strategiją:</span><span class="sxs-lookup"><span data-stu-id="0b827-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="0b827-109">Atnaujinkite vartotojo bendro naudojimo strategiją.</span><span class="sxs-lookup"><span data-stu-id="0b827-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="0b827-110">Jei norite tai padaryti, atlikite tokius veiksmus:</span><span class="sxs-lookup"><span data-stu-id="0b827-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="0b827-111">Atidarykite "Exchange" administravimo centrą.</span><span class="sxs-lookup"><span data-stu-id="0b827-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="0b827-112">Spustelėkite **organizacija**, tada dukart spustelėkite strategiją, priskirtą vartotojui pagal **atskirą bendrą naudojimą**.</span><span class="sxs-lookup"><span data-stu-id="0b827-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="0b827-113">Tai strategija, kuri buvo grąžinta atliekant 2 veiksmą.</span><span class="sxs-lookup"><span data-stu-id="0b827-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="0b827-114">Puslapyje bendrinimo taisyklės pasirinkite kalendoriaus bendrinimo lygį, kurį norite leisti dalyje nurodykite, kurią **informaciją norite bendrinti**; spustelėkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="0b827-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="0b827-115">Daugiau informacijos rasite: ["strategija neleidžia šiuo lygiu suteikti teises vienam ar daugiau gavėjo (-ų)" klaida, kai vartotojas bando bendrinti kalendorių](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="0b827-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
