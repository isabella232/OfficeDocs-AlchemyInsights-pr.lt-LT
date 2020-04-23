---
title: "\"Office 365\" išplėstinės apsaugos nuo grėsmių (ATP) trikčių šalinimas"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766753"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="51125-102">"Office 365" ATP trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="51125-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="51125-103">**Pranešimas vėlavimas su elektroninio pašto pranešimų pristatymo?**</span><span class="sxs-lookup"><span data-stu-id="51125-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="51125-104">Išbandykite parinktį Dinaminis pristatymas ATP saugių priedų strategijoms.</span><span class="sxs-lookup"><span data-stu-id="51125-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="51125-105">Tai padės išvengti el. laiškų pristatymo delsos, tuo pačiu apsaugant gavėjus nuo kenkėjiškų failų.</span><span class="sxs-lookup"><span data-stu-id="51125-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="51125-106">**Ar norite pranešti apie klaidingus teigiamus ar klaidingus negatyvus?**</span><span class="sxs-lookup"><span data-stu-id="51125-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="51125-107">Naudokite šį saitą norėdami pateikti failą analizei:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="51125-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="51125-108">**Ar žinote, kad galite įjungti ATP Saugių nuorodų apsaugą el. Laiškams, siunčiamiems tarp jūsų organizacijos žmonių?**</span><span class="sxs-lookup"><span data-stu-id="51125-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="51125-109">Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="51125-109">Follow these steps:</span></span>
    1. <span data-ttu-id="51125-110">Eikite https://protection.office.comį ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="51125-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="51125-111">Eikite į **Grėsmių valdymo** > **strategijos** > **saugios nuorodos**.</span><span class="sxs-lookup"><span data-stu-id="51125-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="51125-112">Dalyje **Strategijos, taikomos konkretiems gavėjams,** redaguokite (arba įtraukite) strategiją.</span><span class="sxs-lookup"><span data-stu-id="51125-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="51125-113">Pasirinkite **Taikyti saugius saitus organizacijos siunčiamiems pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="51125-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="51125-114">Įrašykite politiką ir leiskite apie 30 minučių, kad pakeitimai veiktų per duomenų centrą.</span><span class="sxs-lookup"><span data-stu-id="51125-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="51125-115">Norėdami gauti daugiau pagalbos dėl ATP, [žr.](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="51125-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>