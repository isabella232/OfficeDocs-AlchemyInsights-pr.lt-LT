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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833083"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>"Microsoft 365" programų "Atsiprašome, kita jūsų organizacijos paskyra jau yra prisijungusi" taisymo pranešimas

Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:

- Pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą, naudodami "Windows" > **"Access" darbo arba mokymo įstaigos**.
- [Išvalykite "Office"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kredencialus naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** "Office 2016" registro keliai pakeisti į 16.0. (pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atidarykite "Office" programą, **pasirinkite**  >  **Failo paskyra**  >  **Atsijungti**. Tada prisijunkite naudodami vartotojo paskyrą su galiojančia licencija. Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Daugiau informacijos žr. "Atsiprašome, kita jūsų organizacijos paskyra jau [yra prisijungusi šiame kompiuteryje" "Office".](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)