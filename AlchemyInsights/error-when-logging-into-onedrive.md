---
title: 0x8004de40 klaida paleidžiant "OneDrive"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946587"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 klaida paleidžiant "OneDrive"

Jei gaunate klaidos **pranešimą 0x8004de40 prisijungiant** prie "OneDrive", iš naujo paleiskite kompiuterį prisijungę prie darbo arba mokymo įstaigos domeno. Jei gaunate šią klaidą iš naujo paleidę kompiuterį, pabandykite tai padaryti prisijungę prie savo darbo arba mokymo įstaigos domeno:

1. Spustelėkite Pradėti ir ieškos **lauke įveskite cmd** **arba komandinę**  eilutę, dešiniuoju pelės mygtuku spustelėkite komandinės eilutės taikomąją programą ir pasirinkite  **Vykdyti administratoriaus teisėmis**. Jei būsite paraginti įvesti administratoriaus slaptažodį arba patvirtinti, įveskite slaptažodį arba spustelėkite **Leisti**.  

2. Komandinės eilutės lange įveskite **dsregcmd /leave**  ir palaukite, kol bus baigta komanda. Tada įveskite **dsregcmd /join ir** palaukite, kol bus baigta komanda.
3. Iš naujo paleiskite kompiuterį.
