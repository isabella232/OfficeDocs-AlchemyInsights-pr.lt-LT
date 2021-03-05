---
title: Apie "Exchange Server" saugos naujinimus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481950"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="076da-102">Apie "Exchange Server" saugos naujinimus</span><span class="sxs-lookup"><span data-stu-id="076da-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="076da-103">"Microsoft" išleido svarbius saugos naujinimus, skirtus "Exchange Server" vietoje.</span><span class="sxs-lookup"><span data-stu-id="076da-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="076da-104">Pažeistos serverio versijos yra visi "Exchange Server 2010", "2013", "2016" ir "2019" naujinimo lygiai.</span><span class="sxs-lookup"><span data-stu-id="076da-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="076da-105">"Exchange Online" nepaveikė, bet jei turite kai kuriuos vietinius "Exchange" serverius dėl Hibridinės konfigūracijos, jie gali būti pažeidžiami.</span><span class="sxs-lookup"><span data-stu-id="076da-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="076da-106">Norėdami atnaujinti vietinius serverius, turėsite vykdyti bent šias "Exchange" versijas:</span><span class="sxs-lookup"><span data-stu-id="076da-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="076da-107">"Exchange 2010" 3 pakeitimų paketas</span><span class="sxs-lookup"><span data-stu-id="076da-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="076da-108">"Exchange Server" 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="076da-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="076da-109">"Exchange Server" 2016 CU 19 arba CU 18</span><span class="sxs-lookup"><span data-stu-id="076da-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="076da-110">"Exchange Server" 2019 CU 8 arba CU 7</span><span class="sxs-lookup"><span data-stu-id="076da-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="076da-111">Žiūrėkite šį skelbimą apie taisymų vietą: [išleista: kovo 2021 "Exchange Server" saugos naujinimai](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="076da-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="076da-112">**Svarbios pastabos:**</span><span class="sxs-lookup"><span data-stu-id="076da-112">**Important notes:**</span></span>

<span data-ttu-id="076da-113">Naujinimų diegimas neveiks, jei jūsų vietiniai serveriai nevykdo reikalingų "Exchange" versijų, kaip nurodyta aukščiau esančiame sąraše.</span><span class="sxs-lookup"><span data-stu-id="076da-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="076da-114">Jei naujinimus diegiate rankiniu būdu, perskaitykite "žinomos problemos" naujinimo KB straipsnių dalyje svarbią informaciją.</span><span class="sxs-lookup"><span data-stu-id="076da-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="076da-115">Saugos naujinimai turi būti paleisti naudojant "CMD/PowerShell" raginimą!</span><span class="sxs-lookup"><span data-stu-id="076da-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
