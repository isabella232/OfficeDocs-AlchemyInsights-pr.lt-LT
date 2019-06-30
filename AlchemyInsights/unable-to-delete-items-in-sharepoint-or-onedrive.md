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
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366541"
---
# <a name="unable-to-delete-items"></a>Neįmanoma panaikinti elementai

Kyla problemų panaikinus elementus?

- Visada įsitikinkite, kad turite [reikiamas teises](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) naikinti elementą arba [svetainių rinkinio administratorius](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) bandymas pašalinti elementą.

- Užtikrinti, kad ten yra [saugojimo strategijos](https://docs.microsoft.com/office365/securitycompliance/retention-policies) nustatymas elementą.

- Užtikrinti prekės nėra [paėmęs](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kitas vartotojas.

- Galiausiai, administratoriai gali naudoti [SharePoint modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kurioje yra biblioteka, "PowerShell" komandas, kurios leidžia jums atlikti sudėtingas valdymo veiksmus, pvz., jėga, naikinami užsispyręs elementai.
- [PNP failą pašalinti](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Pašalinti PNP aplanką](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Pašalinti PNP sąrašo elementą.](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Pašalinti PNP sąrašas](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Pašalinti PNP lauko (stulpelio)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)