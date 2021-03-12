---
title: Prisijungimo prie "Microsoft 365" programų problemos
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709114"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>"Microsoft 365" taikomųjų programų taisymas pranešimas "jūsų kompiuterio patikimos platformos modulis neveikia tinkamai"

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir " [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)" naujinimus.
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) naudodami "Windows" Kredencialų tvarkytuvą.<br/>
    **Pastaba:** "Office 2016" registro keliai pakeisti į "16,0". (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Išbandykite [vartotojų atkūrimo procesą](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , kad išspręstumėte patikimos platformos modulio (TPM) triktis.
- Nustatykite EnableADAL = 0 atlikdami šiuos veiksmus:  
    1. Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką pradėti, pasirinkite **vykdyti**, įveskite **regedit**, tada pasirinkite **gerai**.
    2. Pasirinkite **taip** , kad leistumėte registro rengyklę atlikti savo įrenginio keitimą.
    3. Registro rengyklėje įtraukite **Enableadal** DWORD reikšmę su parametru **0** dalyje HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Daugiau informacijos ieškokite [prisijungimo problemų prisijungiant, atnaujinus į "Office 2016" komponavimo versiją 16.0.7967 "Windows 10"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).