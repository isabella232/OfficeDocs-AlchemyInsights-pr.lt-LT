---
title: Klaidos 0x8004de40 taisymas "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716036"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Klaidos 0x8004de40 taisymas "OneDrive"

Jei su "OneDrive" gaunate klaidos pranešimą 0x8004de40:

- Perkraukite paveiktą kompiuterį, kai prijungtas prie acitve katalogo domeno.
- Jei iš naujo neišsprendžia problemos, atjunkite ir vėl prisijunkite prie įrenginio iš "Azure AD". 

**Pastaba:** atlikdami šiuos veiksmus turėtumėte būti įmonės tinkle. Neatlikite šių veiksmų, kai negalite prisijungti prie įmonės infrastruktūros (pvz., keliaudami). 

- Atidarykite didesnių teisių komandinę eilutę. 
- Norėdami atidaryti didesnių teisių komandų eilutę, spustelėkite - **Pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**, tada spustelėkite **Paleisti administratoriaus teisėmis**.
- Įveskite *dsregcmd /leave* ir paspauskite **Enter**.
- Baigę įveskite *dsregcmd /join* ir paspauskite **Enter**.
- Baigę uždarykite komandinę eilutę.
- Perkraukite kompiuterį ir prisijunkite prie "OneDrive".