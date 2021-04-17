---
title: Prisijungimo prie "Microsoft 365" programų problemos
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
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833012"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Pranešimas "Microsoft 365" programų "Jūsų kompiuterio patikimos platformos modulis veikia netinkamai" taisymas

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Įdiekite naujausius ["Windows" ir "Office"](https://support.microsoft.com/help/4027667/windows-10-update) [naujinimus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Išvalykite "Office"](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) kredencialus naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** "Office 2016" registro keliai pakeisti į 16.0. (pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Išbandykite [vartotojo atkūrimo procesą,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) kad išspręstų patikimos platformos modulio (TPM) triktis.
- Nustatykite EnableADAL = 0, atlikite šiuos veiksmus:  
    1. Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką Pradžia, **pasirinkite Vykdyti**, **įveskite regedit**, tada pasirinkite **Gerai**.
    2. Pasirinkite **Taip,** kad registro rengyklė galėtų atlikti įrenginio keitimus.
    3. Registro rengyklėje įtraukite **"EnableADAL"** DWORD reikšmę su **parametru 0 dalyje** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Daugiau informacijos žr. Prisijungimo problemos atnaujinus į ["Office 2016" komponavimo versiją 16.0.7967 sistemoje "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)