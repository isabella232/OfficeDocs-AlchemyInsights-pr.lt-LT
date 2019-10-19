---
title: "\"SharePoint\" arba \"OneDrive\" prieigos ribojimas"
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551459"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="dc2eb-102">"SharePoint" arba "OneDrive" prieigos ribojimas</span><span class="sxs-lookup"><span data-stu-id="dc2eb-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="dc2eb-103">Programoje "SharePoint" ir "OneDrive" apribojate prieigą prie elementų, pvz., failų, aplankų ir sąrašų, suteikdami prieigą tik prie grupių ar asmenų, kuriuos norite pasiekti.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="dc2eb-104">Pagal numatytuosius nustatymus "SharePoint" teisės paveldimos aukštesniu hierarchijos atveju.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="dc2eb-105">Taigi failas paveldi savo teises iš aplanko, kuris paveldi savo teises iš bibliotekos, kuri paveldi savo teises iš svetainės.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="dc2eb-106">Galite bendrinti aukštesniu lygiu (pvz., bendrai naudodami visą svetainę), tada nutraukti paveldimumą, jei nenorite bendrinti visų svetainės elementų.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="dc2eb-107">Tačiau nerekomenduojame to daryti, nes tai leidžia išlaikyti daugiau sudėtingų ir painesnių teisių ateityje.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="dc2eb-108">Štai ką galite padaryti vietoj:</span><span class="sxs-lookup"><span data-stu-id="dc2eb-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="dc2eb-109">Jei, pavyzdžiui, norite bendrinti visą aplanko turinį, išskyrus vieną failą, perkelkite tą failą į naują vietą, kuri nėra bendrinama.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="dc2eb-110">Jei aplanke yra du poaplankiai ir norite bendrinti vieną poaplankį su A ir B grupėmis ir leisti tik grupės A prieigą prie antrojo poaplankio, bendrai naudoti pirminį aplanką su grupe A ir į pirmąjį poaplankį įtraukti B grupę.</span><span class="sxs-lookup"><span data-stu-id="dc2eb-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="dc2eb-111">Failo arba aplanko bendrinimo sustabdymas</span><span class="sxs-lookup"><span data-stu-id="dc2eb-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

