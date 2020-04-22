---
title: Prieigos ribojimas "SharePoint" arba "OneDrive"
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715892"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="93ef5-102">Prieigos ribojimas "SharePoint" arba "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="93ef5-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="93ef5-103">"SharePoint" ir "OneDrive" ribojate prieigą prie elementų, pvz., failų, aplankų ir sąrašų, suteikdami prieigą tik grupėms ar asmenims, kuriuos norite pasiekti.</span><span class="sxs-lookup"><span data-stu-id="93ef5-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="93ef5-104">Pagal numatytuosius nustatymus "SharePoint" teisės hierarchijoje paveldimos iš aukštesnio lygio.</span><span class="sxs-lookup"><span data-stu-id="93ef5-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="93ef5-105">Taigi failas paveldi savo teises iš aplanko, kuris paveldi jo teises iš bibliotekos, kuri paveldi jo teises iš svetainės.</span><span class="sxs-lookup"><span data-stu-id="93ef5-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="93ef5-106">Galite bendrinti aukštesniu lygiu (pvz., bendrindami visą svetainę) ir tada nutraukti paveldimumą, jei nenorite bendrinti visų svetainės elementų.</span><span class="sxs-lookup"><span data-stu-id="93ef5-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="93ef5-107">Tačiau mes to nerekomenduojame, nes dėl to ateityje teisės tampa sudėtingesnės ir painesnės.</span><span class="sxs-lookup"><span data-stu-id="93ef5-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="93ef5-108">Štai ką galėtumėte padaryti vietoj:</span><span class="sxs-lookup"><span data-stu-id="93ef5-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="93ef5-109">Pavyzdžiui, jei norite bendrinti visą aplanko turinį, išskyrus vieną jame esantį failą, perkelkite jį į naują vietą, kuri nėra bendrinama.</span><span class="sxs-lookup"><span data-stu-id="93ef5-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="93ef5-110">Jei aplanke yra du poaplankiai ir norite bendrinti vieną poaplankį su A ir B grupėmis ir leisti tik grupę A prieigą prie antrojo poaplankio, bendrinkite pirminį aplanką su grupe A ir įtraukite Grupę B į pirmąjį poaplankį.</span><span class="sxs-lookup"><span data-stu-id="93ef5-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="93ef5-111">Failo arba aplanko bendrinimo sustabdymas</span><span class="sxs-lookup"><span data-stu-id="93ef5-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

