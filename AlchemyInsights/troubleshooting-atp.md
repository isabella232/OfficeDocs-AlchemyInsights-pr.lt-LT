---
title: "\"Microsoft Defender\" trikčių diagnostika \"Office 365\""
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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801451"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="81208-102">"Microsoft Defender" trikčių diagnostika "Office 365"</span><span class="sxs-lookup"><span data-stu-id="81208-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="81208-103">Ar pastebite vėlavimą pranešimo pristatymui?</span><span class="sxs-lookup"><span data-stu-id="81208-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="81208-104">Naudokite [dinaminio pristatymo](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) parinktį "ATP Safe" priedų strategijoje.</span><span class="sxs-lookup"><span data-stu-id="81208-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="81208-105">Tai padės išvengti pranešimo gaišaties saugant gavėjus iš kenkėjiškų failų.</span><span class="sxs-lookup"><span data-stu-id="81208-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="81208-106">Ar norite pranešti apie neteisingus teigiamus rezultatus arba neteisingus negatyvus "Microsoft"?</span><span class="sxs-lookup"><span data-stu-id="81208-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="81208-107">Naudokite šį [saitą](https://www.microsoft.com/wdsi/filesubmission/) , jei norite pateikti analizei skirtus failus.</span><span class="sxs-lookup"><span data-stu-id="81208-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="81208-108">Ar žinojote, kad galite įgalinti saugių saitų apsaugą vidiniame el. laiške, siunčiamame tarp jūsų organizacijos gavėjų?</span><span class="sxs-lookup"><span data-stu-id="81208-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="81208-109">Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="81208-109">Follow these steps:</span></span>

  1. <span data-ttu-id="81208-110">Eikite į [https://protection.office.com](https://protection.office.com) ir prisijunkite naudodami visuotinio administratoriaus arba saugos administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="81208-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="81208-111">Kairiojoje naršymo srityje, dalyje **grėsmių valdymas** pasirinkite **strategijos** \> **saugūs saitai** .</span><span class="sxs-lookup"><span data-stu-id="81208-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="81208-112">Strategijų, **kurios taikomos visai organizacijai** , pasirinkite strategiją ir spustelėkite **Redaguoti** .</span><span class="sxs-lookup"><span data-stu-id="81208-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="81208-113">Dalyje **Parametrai** įgalinkite **taikyti saugius saitus organizacijos siunčiamuose pranešimuose** .</span><span class="sxs-lookup"><span data-stu-id="81208-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
