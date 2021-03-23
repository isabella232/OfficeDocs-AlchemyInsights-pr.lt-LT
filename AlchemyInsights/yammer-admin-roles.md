---
title: Apie "Yammer" administratoriai
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/22/2021
ms.locfileid: "51036718"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="b8821-102">Apie "Yammer" administratoriai</span><span class="sxs-lookup"><span data-stu-id="b8821-102">About Yammer admins</span></span>

<span data-ttu-id="b8821-103">**Tinklo administratoriai**</span><span class="sxs-lookup"><span data-stu-id="b8821-103">**Network admins**</span></span>

<span data-ttu-id="b8821-104">Visuotiniai administratoriai automatiškai skatinami į patvirtintą administratoriaus vaidmenį "Yammer" tinkle.</span><span class="sxs-lookup"><span data-stu-id="b8821-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="b8821-105">Toliau nurodytais atvejais ši akcija gali būti netinkamai:</span><span class="sxs-lookup"><span data-stu-id="b8821-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="b8821-106">Yra keli "Yammer" tinklai, o administratorius yra pasirašęs su netinkamu.</span><span class="sxs-lookup"><span data-stu-id="b8821-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="b8821-107">Norint patekti į vieną "Yammer" tinklą reikia [tinklo konsolidacijos](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) .</span><span class="sxs-lookup"><span data-stu-id="b8821-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="b8821-108">Naudojamas "Azure PIM".</span><span class="sxs-lookup"><span data-stu-id="b8821-108">Azure PIM is being used.</span></span> <span data-ttu-id="b8821-109">Vartotojas negali būti paaukštintas į visuotinio administratoriaus pakankamai ilgą laiką, kad būtų skatinama.</span><span class="sxs-lookup"><span data-stu-id="b8821-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="b8821-110">Būsimasis "Yammer" naujinimas gali išspręsti šią problemą, tačiau geriausia, kad vartotojai būtų skatinami naudoti visuotinio administravimo neautomatiškai.</span><span class="sxs-lookup"><span data-stu-id="b8821-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="b8821-111">Sinchronizavimo problema yra "Yammer" tinkle.</span><span class="sxs-lookup"><span data-stu-id="b8821-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="b8821-112">Šiuo atveju bus reikalaujama palaikymo užklausa tolesniam tyrimui.</span><span class="sxs-lookup"><span data-stu-id="b8821-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="b8821-113">Daugiau informacijos apie "Yammer" administravimo vaidmenis rasite " [Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)" administratorių valdymas.</span><span class="sxs-lookup"><span data-stu-id="b8821-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="b8821-114">**Grupės Administratoriai**</span><span class="sxs-lookup"><span data-stu-id="b8821-114">**Group admins**</span></span>

<span data-ttu-id="b8821-115">Grupės Administratoriai, skirti "Microsoft 365 Connected Groups", sinchronizuojami su grupės nariais iš "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="b8821-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="b8821-116">Didelėms grupėms Šis sinchronizavimas gali užtrukti ilgą laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="b8821-116">For large groups, this sync can take an extended period.</span></span>
