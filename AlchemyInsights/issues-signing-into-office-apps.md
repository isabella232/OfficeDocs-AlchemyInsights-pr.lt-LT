---
title: Prisijungimo prie "Microsoft 365" programėlių problemos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579873"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>"Microsoft 365" programėlių "Kompiuterio patikimos platformos modulis veikia netinkamai" nustatymas

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir ["Office"](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)naujinimus .
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0. (Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Pabandykite [vartotojo atkūrimo procesą,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) norėdami išspręsti patikimos platformos modulio (TPM) triktys.
- Nustatykite EnableADAL = 0 atlikdami šiuos veiksmus:  
    1. Dešiniuoju pelės mygtuku spustelėkite mygtuką Windows pradėti, pasirinkite **Vykdyti**, įveskite **regedit**, tada pasirinkite **Gerai**.
    2. Pasirinkite **Taip,** kad leistumėte registro rengyklei keisti įrenginį.
    3. Registro rengyklėje įtraukite **EnableADAL** DWORD reikšmę su parametru **0** pagal HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Jei norite gauti daugiau informacijos, peržiūrėkite [ryšio problemos prisijungimo atnaujinus į Office 2016 komponavimo versijos 16.0.7967 "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)