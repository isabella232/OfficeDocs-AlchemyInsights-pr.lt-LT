---
title: Prisijungimo prie "Microsoft 365" problemos
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986899"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Pranešimų Microsoft 365 "Jūsų kompiuterio patikimos platformos modulis veikia netinkamai"

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) [ir "Office" naujinimus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Išvalykite Office kredencialus](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvą.<br/>
    **Pastaba:** 2016 m. Office keliai pakeisti į 16.0. (ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Išbandykite [vartotojo atkūrimo procesą,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) kad išspręstų patikimos platformos modulio (TPM) triktis.
- Nustatykite EnableADAL = 0, atlikite šiuos veiksmus:  
    1. Dešiniuoju pelės mygtuku Windows mygtuką Pradžia, **pasirinkite Vykdyti**, įveskite **regedit**, tada pasirinkite **Gerai**.
    2. Pasirinkite **Taip,** kad registro rengyklė galėtų atlikti įrenginio keitimus.
    3. Registro rengyklėje įtraukite **"EnableADAL"** DWORD reikšmę su **parametru 0 dalyje** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Daugiau informacijos žr. Prisijungimo problemos atnaujinus į ["Office 2016" komponavimo versiją 16.0.7967" Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).