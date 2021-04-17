---
title: "\"Microsoft 365\" programų taisymo atsiprašome, mes turime laikinų serverio problemų pranešimą"
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835279"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>"Microsoft 365" programų taisymo pranešimas "Atsiprašome, kyla laikinų serverio problemų"

Jei gaunate šį pranešimą, bandykite atlikti šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Microsoft 365" programų. Žr. [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite **į Pradėti**  >  **vykdyti**, tada įveskite **services.msc**. Įsitikinkite, kad visos šios tarnybos veikia:
    - Tinklo prijungtų įrenginių automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vietos žinomumas
    - "Windows" įvykių žurnalas

Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti. Jei kyla problemų pradedant tarnybą, vykdykite šią komandą atidarydami komandinę eilutę su didesnėmis teisėmis:

**sfc /scannow**

Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.

Išsamios informacijos ieškokite ["Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai suaktyvinsite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).