---
title: Klaidos sprendimas 0x8004de40 "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745138"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Klaidos sprendimas 0x8004de40 "OneDrive"

Jei gavote 0x8004de40 klaidą su "OneDrive":

- Iš naujo paleiskite paveiktą kompiuterį, kai esate prisijungę prie "Acitve" katalogų domeno.
- Jei perkrovimas nepadeda išspręsti problemos, prisijunkite prie įrenginio naudodami "Azure AD" ir vėl prisijunkite prie jo. 

**Pastaba**: turite būti įmonės tinkle atlikdami šiuos veiksmus. Neatlikite šių veiksmų, kai negalėsite prisijungti prie savo įmonės infrastruktūros (pvz., keliaudami). 

- Atidarykite didesnių teisių komandinę eilutę. 
- Norėdami atidaryti didesnių teisių komandinę eilutę, spustelėkite – **pradėti**, dešiniuoju pelės mygtuku spustelėkite **Komandinė eilutė**, tada spustelėkite **paleisti administratoriaus**teisėmis.
- Įveskite *dsregcmd/Leave* ir paspauskite " **įvesti**".
- Baigę įveskite *dsregcmd/Join* ir paspauskite klavišą " **įvesti**".
- Baigę uždarykite komandinę eilutę.
- Iš naujo paleiskite kompiuterį ir Prisiregistruokite prie "OneDrive".