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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511120"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="6da74-102">"Office 365" ATP trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="6da74-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="6da74-103">**Pranešimas vėlavimas su elektroninio pašto pranešimų pristatymo?**</span><span class="sxs-lookup"><span data-stu-id="6da74-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="6da74-104">Išbandykite parinktį Dinaminis pristatymas ATP saugių priedų strategijoms.</span><span class="sxs-lookup"><span data-stu-id="6da74-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="6da74-105">Tai padės išvengti el. laiškų pristatymo delsos, tuo pačiu apsaugant gavėjus nuo kenkėjiškų failų.</span><span class="sxs-lookup"><span data-stu-id="6da74-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="6da74-106">**Ar norite pranešti apie klaidingus teigiamus ar klaidingus negatyvus?**</span><span class="sxs-lookup"><span data-stu-id="6da74-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="6da74-107">Naudokite šį saitą norėdami pateikti failą analizei:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="6da74-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="6da74-108">**Ar žinote, kad galite įjungti ATP Saugių nuorodų apsaugą el. Laiškams, siunčiamiems tarp jūsų organizacijos žmonių?**</span><span class="sxs-lookup"><span data-stu-id="6da74-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="6da74-109">Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="6da74-109">Follow these steps:</span></span>
    1. <span data-ttu-id="6da74-110">Eikite į https://protection.office.com ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="6da74-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="6da74-111">Eikite į **Grėsmių valdymo**  >  **strategijos**  >  **saugios nuorodos**.</span><span class="sxs-lookup"><span data-stu-id="6da74-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="6da74-112">Dalyje **Strategijos, taikomos konkretiems gavėjams,** redaguokite (arba įtraukite) strategiją.</span><span class="sxs-lookup"><span data-stu-id="6da74-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="6da74-113">Pasirinkite **Taikyti saugius saitus organizacijos siunčiamiems pranešimams**.</span><span class="sxs-lookup"><span data-stu-id="6da74-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="6da74-114">Įrašykite politiką ir leiskite apie 30 minučių, kad pakeitimai veiktų per duomenų centrą.</span><span class="sxs-lookup"><span data-stu-id="6da74-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="6da74-115">Norėdami gauti daugiau pagalbos dėl ATP, [žr.](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="6da74-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>