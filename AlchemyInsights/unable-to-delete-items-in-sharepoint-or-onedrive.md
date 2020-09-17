---
title: Nepavyksta panaikinti elementų "SharePoint" arba "OneDrive"
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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806119"
---
# <a name="unable-to-delete-items"></a>Nepavyksta panaikinti elementų

Dėl išsaugojimo strategijų, reikia išjungti arba pašalinti atitinkamą sulaikymą, dėl kurio kyla ši problema. Pašalinus saugojimo strategiją arba sulaikymą, gali užtrukti iki 24 valandų, kol įsigalios pakeitimai. Įsitikinkite, kad elemente nėra [išsaugojimo strategijos](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) nustatymų.

Svetainė galėjo viršyti saugyklos limitą, padidinti [svetainės kvotą](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ir panaikinti elementą.

Įsitikinkite, kad elementas [nepaimtas](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) į kitą vartotoją.

Galiausiai administratoriai gali naudoti " [SharePoint" modelius ir praktiką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kuriuose yra "PowerShell" komandų biblioteka, leidžianti atlikti sudėtingus valdymo veiksmus, pvz., priverčiančius panaikinti elementus.
- [Pašalinkite PNP failą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Pašalinkite PNP aplanką](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP sąrašo elemento šalinimas](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Pašalinti PNP sąrašą](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Šalinti PNP lauką (stulpelis)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)