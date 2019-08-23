---
title: Neįmanoma panaikinti elementus SharePoint arba "OneDrive"
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558661"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="31391-102">Neįmanoma panaikinti elementai</span><span class="sxs-lookup"><span data-stu-id="31391-102">Unable to delete items</span></span>

<span data-ttu-id="31391-103">Kyla problemų naikinami SharePoint elementai?</span><span class="sxs-lookup"><span data-stu-id="31391-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="31391-104">Visada įsitikinkite, kad turite [reikiamas teises](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) naikinti elementą arba [svetainių rinkinio administratorius](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) bandymas pašalinti elementą.</span><span class="sxs-lookup"><span data-stu-id="31391-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="31391-105">Užtikrinti, kad ten yra [saugojimo strategijos](https://docs.microsoft.com/office365/securitycompliance/retention-policies) nustatymas elementą.</span><span class="sxs-lookup"><span data-stu-id="31391-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="31391-106">Užtikrinti prekės nėra [paėmęs](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kitas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="31391-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="31391-107">Galiausiai, administratoriai gali naudoti [SharePoint modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kurioje yra biblioteka, "PowerShell" komandas, kurios leidžia jums atlikti sudėtingas valdymo veiksmus, pvz., jėga, naikinami užsispyręs elementai.</span><span class="sxs-lookup"><span data-stu-id="31391-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="31391-108">PNP failą pašalinti</span><span class="sxs-lookup"><span data-stu-id="31391-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="31391-109">Pašalinti PNP aplanką</span><span class="sxs-lookup"><span data-stu-id="31391-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="31391-110">Pašalinti PNP sąrašo elementą.</span><span class="sxs-lookup"><span data-stu-id="31391-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="31391-111">Pašalinti PNP sąrašas</span><span class="sxs-lookup"><span data-stu-id="31391-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="31391-112">Pašalinti PNP lauko (stulpelio)</span><span class="sxs-lookup"><span data-stu-id="31391-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)