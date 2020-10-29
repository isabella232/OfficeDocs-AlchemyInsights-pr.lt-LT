---
title: "\"Microsoft Defender\" trikčių diagnostika \"Office 365\" (ATP)"
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801415"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c41e5-102">"Office 365 ATP" problemų šalinimas</span><span class="sxs-lookup"><span data-stu-id="c41e5-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c41e5-103">**Pranešimas delsa su el. laiško pristatymu** ?</span><span class="sxs-lookup"><span data-stu-id="c41e5-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="c41e5-104">Bandykite naudoti dinaminio pristatymo parinktį, skirtą "ATP" saugos priedų strategijoms.</span><span class="sxs-lookup"><span data-stu-id="c41e5-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c41e5-105">Taip išvengsite el. laiško pristatymo uždelsimo, nes apsaugodami gavėjus nuo kenkėjiškų failų.</span><span class="sxs-lookup"><span data-stu-id="c41e5-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c41e5-106">Ar norite **pranešti apie neteisingus teigiamus rezultatus ar neteisingus negatyvus** ?</span><span class="sxs-lookup"><span data-stu-id="c41e5-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="c41e5-107">Naudokite šį saitą, jei norite pateikti savo failą analizei: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c41e5-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c41e5-108">**Ar žinojote, kad galite įjungti ATP saugos saitų apsaugą el. paštui, siunčiamame tarp jūsų organizacijos žmonių** ?</span><span class="sxs-lookup"><span data-stu-id="c41e5-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="c41e5-109">Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="c41e5-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c41e5-110">Eikite į https://protection.office.com ir prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="c41e5-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c41e5-111">Eikite į **grėsmių valdymo**  >  **strategijos**  >  **saugos saitai** .</span><span class="sxs-lookup"><span data-stu-id="c41e5-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="c41e5-112">Dalyje strategijos **, taikomos konkretiems gavėjams** , redaguokite (arba įtraukite) strategiją.</span><span class="sxs-lookup"><span data-stu-id="c41e5-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c41e5-113">Pasirinkite **taikyti saugius saitus su pranešimais, siunčiamuose organizacijoje** .</span><span class="sxs-lookup"><span data-stu-id="c41e5-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="c41e5-114">Įrašykite savo strategiją ir leiskite apie 30 minučių, kol jūsų pokyčiai veiks jūsų duomenų centre.</span><span class="sxs-lookup"><span data-stu-id="c41e5-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c41e5-115">Norėdami gauti daugiau pagalbos dėl ATP, skaitykite ["Microsoft Defender for Office 365"](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="c41e5-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>