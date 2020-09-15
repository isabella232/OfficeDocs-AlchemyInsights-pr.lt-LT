---
title: "\"Office 365\" išplėstinės grėsmės apsaugos trikčių diagnostika"
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658922"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="a5a5f-102">"Office 365" išplėstinės grėsmės apsaugos trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="a5a5f-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="a5a5f-103">Ar pastebite vėlavimą pranešimo pristatymui?</span><span class="sxs-lookup"><span data-stu-id="a5a5f-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="a5a5f-104">Naudokite [dinaminio pristatymo](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) parinktį "ATP Safe" priedų strategijoje.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="a5a5f-105">Tai padės išvengti pranešimo gaišaties saugant gavėjus iš kenkėjiškų failų.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="a5a5f-106">Ar norite pranešti apie neteisingus teigiamus rezultatus arba neteisingus negatyvus "Microsoft"?</span><span class="sxs-lookup"><span data-stu-id="a5a5f-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="a5a5f-107">Naudokite šį [saitą](https://www.microsoft.com/wdsi/filesubmission/) , jei norite pateikti analizei skirtus failus.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="a5a5f-108">Ar žinojote, kad galite įgalinti saugių saitų apsaugą vidiniame el. laiške, siunčiamame tarp jūsų organizacijos gavėjų?</span><span class="sxs-lookup"><span data-stu-id="a5a5f-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="a5a5f-109">Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a5a5f-109">Follow these steps:</span></span>

  1. <span data-ttu-id="a5a5f-110">Eikite į [https://protection.office.com](https://protection.office.com) ir prisijunkite naudodami visuotinio administratoriaus arba saugos administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="a5a5f-111">Kairiojoje naršymo srityje, dalyje **grėsmių valdymas**pasirinkite **strategijos** \> **saugūs saitai**.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="a5a5f-112">Strategijų, **kurios taikomos visai organizacijai** , pasirinkite strategiją ir spustelėkite **Redaguoti**.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="a5a5f-113">Dalyje **Parametrai**įgalinkite **taikyti saugius saitus organizacijos siunčiamuose pranešimuose**.</span><span class="sxs-lookup"><span data-stu-id="a5a5f-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
