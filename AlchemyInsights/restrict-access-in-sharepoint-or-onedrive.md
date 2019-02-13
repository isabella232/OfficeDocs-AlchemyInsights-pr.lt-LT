---
title: Apriboti prieigos SharePoint arba "OneDrive"
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905156"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8667a-102">Apriboti prieigos SharePoint arba "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="8667a-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8667a-p101">SharePoint ir "OneDrive", galite apriboti prieigą prie daiktų, pavyzdžiui, failų, aplankų ir sąrašų suteikiant prieigą tik grupių arba asmenų, kurį norite pasiekti. Pagal numatytuosius nustatymus programoje "SharePoint" teisės paveldimos iš į aukštesnį hierarchijos. Taigi failą savo teises paveldi iš aplanko, kuris savo teises paveldi iš bibliotekos, kuris savo teises paveldi iš svetainės.</span><span class="sxs-lookup"><span data-stu-id="8667a-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="8667a-p102">Galite bendrai naudoti aukštesnio lygio (pvz., dalijantis visą svetainę) ir tada nutraukti paveldimumą, jei nenorite bendrai naudoti visiems svetainėje elementų. Vis dėlto mes nerekomenduojame tai tampa išlaikyti teises sudėtingos ir painios ateityje. Štai ką gali padaryti vietoj:</span><span class="sxs-lookup"><span data-stu-id="8667a-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="8667a-109">Jei, pvz., norite bendrai naudoti visą turinį, išskyrus vieną failą, aplanką perkelti failą į naują vietą, kuri nėra bendrinama.</span><span class="sxs-lookup"><span data-stu-id="8667a-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="8667a-110">Jei turite du poaplankius aplanke, ir jūs norite pasidalinti viena poaplankio su A ir B grupių ir leisti tik A grupės prieigą prie antrojo poaplankį, pasidalinti į aukštesnio lygio aplanką su A grupės ir B grupės įtraukti į pirmą poaplankį.</span><span class="sxs-lookup"><span data-stu-id="8667a-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="8667a-111">Failo ar aplanko bendrinimo sustabdymas</span><span class="sxs-lookup"><span data-stu-id="8667a-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

