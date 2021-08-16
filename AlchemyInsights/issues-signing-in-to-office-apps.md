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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028048"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Pranešimų Microsoft 365 "Atsiprašome, kita jūsų organizacijos paskyra jau yra prisijungusi"

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą, naudodami "Windows Parametrai > **Access" darbo arba mokymo įstaigos**.
- [Išvalykite Office kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvą.<br/>
    **Pastaba:** 2016 m. Office keliai pakeisti į 16.0. (ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atidarykite "Office" programa, pasirinkite **Failo**  >  **paskyra**  >  **Atsijungti**. Tada prisijunkite naudodami vartotojo paskyrą su galiojančia licencija. Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daugiau informacijos žr. ["Atsiprašome,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)kita jūsų organizacijos paskyra jau yra prisijungusi šiame kompiuteryje" Office.