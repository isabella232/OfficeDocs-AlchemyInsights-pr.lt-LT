---
title: "\"Microsoft\" sargybos trikčių šalinimas Office 365"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545276"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="08264-102">"Microsoft" sargybos trikčių šalinimas Office 365</span><span class="sxs-lookup"><span data-stu-id="08264-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="08264-103">**Ar pastebėjote pranešimų pristatymo delsą?**</span><span class="sxs-lookup"><span data-stu-id="08264-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="08264-104">Naudokite parinktį [Dinaminis pristatymas](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) "Microsoft" sargyboje, kad Office 365 Seifas priedų strategiją.</span><span class="sxs-lookup"><span data-stu-id="08264-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="08264-105">Tai padės išvengti pranešimų delsos apsaugant gavėjus nuo kenkėjiškų failų.</span><span class="sxs-lookup"><span data-stu-id="08264-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="08264-106">**Ar norite pranešti "Microsoft" apie klaidingus teigiamus ar klaidingus neigiamus rezultatus?**</span><span class="sxs-lookup"><span data-stu-id="08264-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="08264-107">Naudokite ["Submissions Explorer".](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="08264-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="08264-108">-\*\* Ar žinote, kad galite įgalinti Seifas saitų apsaugą vidiniams el. laiškams, siunčiamiems tarp jūsų organizacijos gavėjų?\*\* Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="08264-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="08264-109">Eikite [https://protection.office.com](https://protection.office.com) ir prisijunkite naudodami visuotinio administratoriaus arba saugos administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="08264-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="08264-110">Kairiojoje naršymo srityje dalyje **Grėsmių valdymas** pasirinkite **Strategijos Seifas** \> **Saitai**.</span><span class="sxs-lookup"><span data-stu-id="08264-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="08264-111">Sekcijoje **Strategijos, kurios taikomos visai organizacijai,** pasirinkite strategiją ir spustelėkite **Redaguoti**.</span><span class="sxs-lookup"><span data-stu-id="08264-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="08264-112">Dalyje **Parametrai** įjunkite **Taikyti saugius saitus organizacijos siunčiamims laiškams**.</span><span class="sxs-lookup"><span data-stu-id="08264-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
