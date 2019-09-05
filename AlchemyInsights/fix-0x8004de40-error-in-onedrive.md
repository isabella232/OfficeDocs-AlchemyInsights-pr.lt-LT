---
title: "\"OneDrive\" klaidos ištaisymas 0x8004de40"
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755856"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>"OneDrive" klaidos ištaisymas 0x8004de40

Jei įvyksta klaida 0x8004de40 su "OneDrive":

- Perkraukite pažeistą kompiuterį, o prijungtas prie jūsų Acitve katalogo domenas.
- Jei iš naujo nepavyksta išspręsti problemos, atsijungti ir prisijungti savo įrenginį iš Azure AD. 

**Pastaba**: atlikdami šiuos veiksmus, turėtumėte būti įmonės tinkle. Neatlikite šių veiksmų, kai negalite prisijungti prie įmonės infrastruktūros (pvz., keliaudami). 

- Atidarykite didesnių teisių komandų eilutę. 
- Norėdami atidaryti didesnių teisių komandų eilutę, spustelėkite **pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**, tada spustelėkite **paleisti administratoriaus teisėmis**.
- Tipo *dsregcmd/atostogos* ir paspauskite **Enter**.
- Baigę įveskite *dsregcmd/Join* ir paspauskite **Enter**.
- Baigę uždarykite komandinę eilutę.
- Perkraukite kompiuterį ir prisijunkite prie OneDrive.