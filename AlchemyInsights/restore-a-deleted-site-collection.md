---
title: Atkurti panaikintą svetainių rinkinį
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301672"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="8bd0d-102">Atkurti panaikintą svetainių rinkinį</span><span class="sxs-lookup"><span data-stu-id="8bd0d-102">Restore a deleted site collection</span></span>

<span data-ttu-id="8bd0d-p101">Kai administratorius panaikina klasikinis svetainių rinkinio, jis yra dedamas į svetainių rinkinio šiukšlinę, kur jis yra laikomas 93 dienų prieš visam laikui panaikinant. Norėdami atkurti svetainių rinkinio:</span><span class="sxs-lookup"><span data-stu-id="8bd0d-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="8bd0d-105">Klasikinis SharePoint administravimo centro, juostelėje spustelėkite **Šiukšlinė** .</span><span class="sxs-lookup"><span data-stu-id="8bd0d-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="8bd0d-106">Pažymėkite žymės langelį šalia svetainių rinkinio, kurį norite atkurti.</span><span class="sxs-lookup"><span data-stu-id="8bd0d-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="8bd0d-107">Spustelėkite **Atkurti panaikintus elementus**.</span><span class="sxs-lookup"><span data-stu-id="8bd0d-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="8bd0d-p102">Norėdami atkurti panaikinto ryšių svetainę, galite naudoti naują SharePoint administravimo centro peržiūra. Priešingu atveju, jums reikia naudoti "PowerShell". Norėdami atkurti svetainę, kuri priklauso "Office 365" grupei, reikia atkurti Exchange administravimo centro grupės. Grupių gali būti atkurta 30 dienų po to, kai jie panaikinti.</span><span class="sxs-lookup"><span data-stu-id="8bd0d-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

