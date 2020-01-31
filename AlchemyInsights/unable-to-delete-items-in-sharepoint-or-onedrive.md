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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571274"
---
# <a name="unable-to-delete-items"></a>Neįmanoma panaikinti elementų

Saugojimo strategijos gali sukelti tai, jums reikia arba išjungti atitinkamą sulaikymą, kuris sukelia šią problemą. Pašalinus saugojimo strategiją arba sulaikymą, gali užtrukti iki 24 valandų, kol pakeitimas įsigalios. Įsitikinkite, kad elemente nėra [saugojimo strategijos](https://docs.microsoft.com/office365/securitycompliance/retention-policies) nustatymo.

Svetainė gali viršyti saugyklos limitą, padidinti [svetainės kvotą](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ir panaikinti elementą.

Įsitikinkite, kad elementas nėra [paimtas](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kitam vartotojui.

Galiausiai administratoriai gali naudoti [SharePoint modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kuriame yra "PowerShell" komandų biblioteka, leidžianti atlikti sudėtingus valdymo veiksmus, pvz., priverstinai naikinti užsispyrusius elementus.
- [Pašalinti PNP failą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Pašalinti PNP aplanką](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Pašalinti PNP sąrašo elementą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP sąrašo pašalinimas](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Pašalinti PNP lauką (stulpelį)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)