---
title: Nepavyksta panaikinti elementų SharePoint arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038525"
---
# <a name="unable-to-delete-items"></a>Nepavyksta panaikinti elementų

- Saugojimo strategijos gali sukelti šią problemą, turite išjungti arba neįtraukti atitinkamo sulaikymo, dėl kurio kyla ši problema. Pašalinus saugojimo strategiją arba sulaikymą, gali užtrukti iki 24 valandų, kad pakeitimas įsigalios. Įsitikinkite, kad nėra [elemento saugojimo](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) strategijos sąrankos.

- Svetainė galėjo viršyti saugyklos limitą, padidinti [svetainės kvotą ir](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) panaikinti elementą.

- Įsitikinkite, kad elementas [nėra paimtas ir užrakintas](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) kitam vartotojui.

- Galiausiai, administratoriai gali [naudoti "SharePoint Patterns and Practices"](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), kurioje yra "PowerShell" komandų biblioteka, kuri leidžia atlikti sudėtingus valdymo veiksmus, pvz., priverstinai panaikinti užsispyrusius elementus.
- [Šalinti PNP failą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Šalinti PNP aplanką](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP sąrašo elemento pašalinimas](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP sąrašo pašalinimas](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Šalinti PNP lauką (stulpelį)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)