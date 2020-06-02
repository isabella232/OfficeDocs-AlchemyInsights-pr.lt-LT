---
title: Neįmanoma panaikinti elementų "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511984"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="25de3-102">Neįmanoma panaikinti elementų</span><span class="sxs-lookup"><span data-stu-id="25de3-102">Unable to delete items</span></span>

<span data-ttu-id="25de3-103">Saugojimo strategijos gali sukelti tai, jums reikia išjungti arba pašalinti atitinkamą sulaikymą, kuris sukelia šią problemą.</span><span class="sxs-lookup"><span data-stu-id="25de3-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="25de3-104">Pašalinus saugojimo strategiją arba sulaikymą, pakeitimas gali įsigalioti iki 24 valandų.</span><span class="sxs-lookup"><span data-stu-id="25de3-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="25de3-105">Įsitikinkite, kad elemente nėra [saugojimo strategijos](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) nustatymo.</span><span class="sxs-lookup"><span data-stu-id="25de3-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="25de3-106">Svetainė galėjo viršyti saugyklos limitą, padidinti [svetainės kvotą](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ir panaikinti elementą.</span><span class="sxs-lookup"><span data-stu-id="25de3-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="25de3-107">Įsitikinkite, kad elementas [nepaimtas](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ir užrakintas kitam vartotojui.</span><span class="sxs-lookup"><span data-stu-id="25de3-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="25de3-108">Galiausiai administratoriai gali naudoti [SharePoint modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), kuriame yra "PowerShell" komandų biblioteka, leidžianti atlikti sudėtingus valdymo veiksmus, pvz., priverstinai naikinant užsispyrusius elementus.</span><span class="sxs-lookup"><span data-stu-id="25de3-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="25de3-109">Šalinti PNP failą</span><span class="sxs-lookup"><span data-stu-id="25de3-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="25de3-110">Šalinti PNP aplanką</span><span class="sxs-lookup"><span data-stu-id="25de3-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="25de3-111">Šalinti PNP sąrašo elementą</span><span class="sxs-lookup"><span data-stu-id="25de3-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="25de3-112">Šalinti PNP sąrašą</span><span class="sxs-lookup"><span data-stu-id="25de3-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="25de3-113">Šalinti PNP lauką (stulpelį)</span><span class="sxs-lookup"><span data-stu-id="25de3-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)