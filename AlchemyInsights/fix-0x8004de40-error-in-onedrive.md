---
title: "\"OneDrive\" klaidos ištaisymas 0x8004de40"
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052045"
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