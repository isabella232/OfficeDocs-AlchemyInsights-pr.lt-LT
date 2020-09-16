---
title: "\"SharePoint\" arba \"OneDrive\" prieigos apribojimas"
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720690"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a1e7c-102">"SharePoint" arba "OneDrive" prieigos apribojimas</span><span class="sxs-lookup"><span data-stu-id="a1e7c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a1e7c-103">Naudodami "SharePoint" ir "OneDrive", galite apriboti prieigą prie elementų, pvz., failų, aplankų ir sąrašų, suteikiančius prieigą tik grupėms arba asmenims, kuriems norite turėti prieigą.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="a1e7c-104">Pagal numatytuosius "SharePoint" teisės hierarchijoje paveldimos iš aukštesnių teisių.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a1e7c-105">Taigi failas paveldi teises iš aplanko, kuris paveldi jo teises iš bibliotekos, kuri paveldi jos teises iš svetainės.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="a1e7c-106">Galite bendrinti aukštesnio lygio (pvz., bendrinant visą svetainę) ir nutraukti paveldėjimą, jei nenorite bendrinti visų svetainės elementų.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="a1e7c-107">Tačiau nerekomenduojame to daryti, nes dėl to ateityje bus lengviau išlaikyti teises ir painios.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="a1e7c-108">Štai ką galite padaryti vietoj:</span><span class="sxs-lookup"><span data-stu-id="a1e7c-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="a1e7c-109">Jei, pvz., norite bendrinti visą aplanko turinį, išskyrus vieną jame esantį failą, perkelkite tą failą į naują vietą, kuri nėra bendrinama.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="a1e7c-110">Jei turite du aplanko poaplankius ir norite bendrinti vieną poaplankį su A ir B grupėmis, o leisti tik grupės prieigą prie antrojo poaplankio, bendrinkite pirminį aplanką su grupe A ir įtraukite B grupę į pirmą poaplankį.</span><span class="sxs-lookup"><span data-stu-id="a1e7c-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="a1e7c-111">Failo arba aplanko bendro naudojimo sustabdymas </span><span class="sxs-lookup"><span data-stu-id="a1e7c-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

