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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744675"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>El. Microsoft 365 "Atsiprašome, kyla laikinų serverio problemų" pranešimas

Pastaba: jei naudojate senesnę "Windows" versiją (pvz., "Windows 7" SP1, "Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2"), naudokite paprastą pataisą, kad įgalintumėte TLS 1.2 kaip numatytuosius parametrus. Daugiau informacijos žr. Naujinimas, kad [įgalintumėte TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jei gaunate šį pranešimą, bandykite atlikti šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie Microsoft 365 programų. Žr. [URL ir IP adresų diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Eikite **į Pradėti**  >  **vykdyti**, tada įveskite **services.msc**. Įsitikinkite, kad visos šios tarnybos veikia:
    - Tinklo prijungtų įrenginių automatinis nustatymas
    - Tinklo sąrašo tarnyba
    - Tinklo vietos žinomumas
    - Windows Įvykių žurnalas

Jei viena iš šių tarnybų neveikia, pabandykite ją paleisti. Jei kyla problemų pradedant tarnybą, vykdykite šią komandą atidarę komandinę eilutę su didesnėmis teisėmis:

**sfc /scannow**

Kai ši komanda bus baigta, paleiskite kompiuterį iš naujo.

Išsamios informacijos žr. ["Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau" klaida, kai suaktyvinsite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).