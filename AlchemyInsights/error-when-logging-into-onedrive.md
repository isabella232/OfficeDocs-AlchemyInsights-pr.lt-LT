---
title: 0x8004de40 klaida paleidžiant "OneDrive"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823111"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 klaida paleidžiant "OneDrive"

Jei gaunate klaidos pranešimą **0x8004de40** , kai prisijungiate prie "OneDrive", iš naujo paleiskite kompiuterį prisijungę prie savo darbo arba mokymo įstaigos domeno. Jei gaunate šią klaidą paleidę kompiuterį iš naujo, Išbandykite tai būdami prisijungę prie savo darbo arba mokymo įstaigos domeno:

1. Spustelėkite pradėti, tada ieškos lauke įveskite **cmd** arba **Komandinė eilutė**  , dešiniuoju pelės mygtuku spustelėkite Komandinė eilutė ir pasirinkite  **paleisti kaip administratoriui** . Jei esate raginami įvesti administratoriaus slaptažodį arba patvirtinti, įveskite slaptažodį arba spustelėkite **leisti** .  

2. Lange Komandinė eilutė įveskite **dsregcmd/Leave**  ir palaukite, kol komanda bus baigta. Tada įveskite **dsregcmd/Join** ir palaukite, kol komanda bus baigta.
3. Iš naujo paleiskite kompiuterį.
