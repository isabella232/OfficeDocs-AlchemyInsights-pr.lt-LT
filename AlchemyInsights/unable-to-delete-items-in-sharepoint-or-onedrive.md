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
# <a name="unable-to-delete-items"></a>Neįmanoma panaikinti elementų

Kyla problemų naikinant "SharePoint" elementus?

- Visada įsitikinkite, kad turite [reikiamas teises](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) naikinti elementą arba [svetainių rinkinio administratorius](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) bando pašalinti elementą.

- Įsitikinkite, kad elemente nėra [saugojimo strategijos](https://docs.microsoft.com/office365/securitycompliance/retention-policies) nustatymo.

- Įsitikinkite, kad elementas nėra [paimtas](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kitam vartotojui.

- Galiausiai administratoriai gali naudoti [SharePoint modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kuriame yra "PowerShell" komandų biblioteka, leidžianti atlikti sudėtingus valdymo veiksmus, pvz., priverstinai naikinti užsispyrusius elementus.
- [Pašalinti PNP failą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Pašalinti PNP aplanką](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Pašalinti PNP sąrašo elementą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP sąrašo pašalinimas](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Pašalinti PNP lauką (stulpelį)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)