---
title: Nepavyksta panaikinti elementus "SharePoint" arba "OneDrive"
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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049525"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="c3879-102">Neįmanoma panaikinti elementų</span><span class="sxs-lookup"><span data-stu-id="c3879-102">Unable to delete items</span></span>

<span data-ttu-id="c3879-103">Kyla problemų naikinant "SharePoint" elementus?</span><span class="sxs-lookup"><span data-stu-id="c3879-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="c3879-104">Visada įsitikinkite, kad turite [reikiamas teises](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) naikinti elementą arba [svetainių rinkinio administratorius](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) bando pašalinti elementą.</span><span class="sxs-lookup"><span data-stu-id="c3879-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="c3879-105">Įsitikinkite, kad elemente nėra [saugojimo strategijos](https://docs.microsoft.com/office365/securitycompliance/retention-policies) nustatymo.</span><span class="sxs-lookup"><span data-stu-id="c3879-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="c3879-106">Įsitikinkite, kad elementas nėra [paimtas](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kitam vartotojui.</span><span class="sxs-lookup"><span data-stu-id="c3879-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="c3879-107">Galiausiai administratoriai gali naudoti [SharePoint modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kuriame yra "PowerShell" komandų biblioteka, leidžianti atlikti sudėtingus valdymo veiksmus, pvz., priverstinai naikinti užsispyrusius elementus.</span><span class="sxs-lookup"><span data-stu-id="c3879-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="c3879-108">Pašalinti PNP failą</span><span class="sxs-lookup"><span data-stu-id="c3879-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="c3879-109">Pašalinti PNP aplanką</span><span class="sxs-lookup"><span data-stu-id="c3879-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="c3879-110">Pašalinti PNP sąrašo elementą</span><span class="sxs-lookup"><span data-stu-id="c3879-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="c3879-111">PNP sąrašo pašalinimas</span><span class="sxs-lookup"><span data-stu-id="c3879-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="c3879-112">Pašalinti PNP lauką (stulpelį)</span><span class="sxs-lookup"><span data-stu-id="c3879-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)