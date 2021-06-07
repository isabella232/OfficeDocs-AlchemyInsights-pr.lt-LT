---
title: "\"Microsoft\" sargybos, kurios galinis taškas yra \"Linux\", našumo problemos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794004"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="d99d5-102">"Microsoft" sargybos, kurios galinis taškas yra "Linux", našumo problemos</span><span class="sxs-lookup"><span data-stu-id="d99d5-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="d99d5-103">Šiame straipsnyje aprašomi veiksmai, kaip nustatyti "Microsoft Defender for Endpoint" veikimo problemas "Linux".</span><span class="sxs-lookup"><span data-stu-id="d99d5-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="d99d5-104">Pirmiausia svarbu patikrinti, ar problema, su kuriomis susiduriate, išspręsta naudojant naujausią [versiją.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="d99d5-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="d99d5-105">Norėdami pradėti tyrimą, žr. ["Microsoft Defender for Endpoint" veikimo trikčių šalinimas "Linux".](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="d99d5-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="d99d5-106">Išimtys</span><span class="sxs-lookup"><span data-stu-id="d99d5-106">Exclusions</span></span>

<span data-ttu-id="d99d5-107">Išimtys gali padėti sumažinti našumo problemas.</span><span class="sxs-lookup"><span data-stu-id="d99d5-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="d99d5-108">Prieš pradėdami peržiūrėkite savo išimtis, kad būtų žinoma ir dokumentuota papildoma rizika.</span><span class="sxs-lookup"><span data-stu-id="d99d5-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="d99d5-109">Daugiau informacijos žr. "Microsoft Defender [for Endpoint" išimčių konfigūravimas ir tikrintas "Linux".](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="d99d5-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="d99d5-110">Jei turite kelis failus& kuriuos norite pašalinti, ir jie visi yra tame pačiame mountpoint, gali būti lengviau pašalinti mountpoint.</span><span class="sxs-lookup"><span data-stu-id="d99d5-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="d99d5-111">Nuo vasario leidimo 101.22.80 galite neįtraukti viso kalno taško.</span><span class="sxs-lookup"><span data-stu-id="d99d5-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="d99d5-112">Pvz., jei /mnt/backup yra mountpoint, galite įtraukti /mnt/backup į neįtrauktų sąrašą vykdydami šią komandą:</span><span class="sxs-lookup"><span data-stu-id="d99d5-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="d99d5-113">**Pastaba:** įtraukus išimtis padidėja pavojus, kad nebus aptikta kenkėjiškų programų, todėl jos turėtų būti tvarkomos ir įgyvendinamos atsargiai.</span><span class="sxs-lookup"><span data-stu-id="d99d5-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="d99d5-114">Reikia pagalbos?</span><span class="sxs-lookup"><span data-stu-id="d99d5-114">Need Help?</span></span>

<span data-ttu-id="d99d5-115">Norėdami jums padėti efektyviausiu būdu, prieš atidarydami palaikymo bylą, surinkite diagnostikos duomenis.</span><span class="sxs-lookup"><span data-stu-id="d99d5-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
