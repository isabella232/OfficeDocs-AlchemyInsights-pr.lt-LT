---
title: "\"Office Apps\" taisymas jūsų abonementas yra blogos būsenos pranešimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969627"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>"Office" programėlių taisymas "klaida" jūsų abonementas yra blogos būsenos "

Norėdami išspręsti šią klaidą, Išbandykite šias parinktis paveiktame kompiuteryje:

- Atidarykite "Office" programėlę, pasirinkite **failo** > **abonemento** > **Atsijungti nuo visų paskyrų**. Vėl prisijunkite naudodami vartotojo abonementą su galiojančia licencija. Išsamesnės informacijos ieškokite [Office aplankuose](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" Kredencialų tvarkytuvą.<br>
  **Pastaba:** Registro keliai Office 2016 pasikeitė į 16,0. Pvz., \Software\Microsoft\Office\16.0\Common\Identity\
- Susijusio kompiuterio, nustatykite EnableADAL = 0, atlikite šiuos veiksmus:  
     1. Dešiniuoju pelės mygtuku spustelėkite mygtuką "Windows" ir pasirinkite **vykdyti**. Lauke **atidaryti** įveskite **regedit**, ir tada pasirinkite **gerai**.
     2. Pasirinkite **taip** Kai paraginama leisti registro rengyklėje atlikti keitimus įrenginyje.
    3. Registro rengyklėje pridėkite EnableADAL DWORD reikšmę su parametr 0 pagal HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Jei klaida įvyksta jungiantis prie "Office 365" naudojant "Office 2013", [įjunkite modernų](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) "Office" kliento autentifikavimą.

Jei norite gauti daugiau informacijos, Sužinokite, [kaip spręsti ne naršyklės programas, kurios negali prisijungti prie Office 365, Azure arba Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

