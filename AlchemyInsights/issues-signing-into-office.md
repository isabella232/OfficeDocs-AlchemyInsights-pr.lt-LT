---
title: Prisijungimo prie "Office" taikomųjų programų problemos
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763009"
---
# <a name="issues-signing-in-to-office-apps"></a>Prisijungimo prie "Office" taikomųjų programų problemos

Norėdami išspręsti prisijungimo problemas, susijusias su "Office" programomis, pabandykite atlikti šiuos veiksmus:

- Pašalinkite visus darbo abonementus, išskyrus paveiktą abonementą, naudodami "Windows" parametrus > **"Access" darbą arba mokyklą**.
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0. (Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atidarykite "Office" programą, pasirinkite > **Atsijungti prie** **failų** > **abonemento**. Tada prisijunkite naudodami vartotojo abonementą su galiojančia licencija. Norėdami rasti išsamios informacijos, žr. [Paskyros programoje „Office“](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Jei naudojate „Mac“, žr. [Negalima prisijungti prie „Office 2016“, skirtos „Mac“](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Jei klaidos įvyksta jungiantis prie "Microsoft 365" naudojant "Office 2013", įgalinkite šiuolaikinės autentifikavimas Office kliento.

Daugiau informacijos rasite:
- [Negalite prisijungti prie "Microsoft 365", "Azure" arba "Intune"](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Ryšio problemos, kai atnaujinate į "Office 2016" komponavimo versijos 16.0.7967 "Windows 10"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Atsiprašome, kitas jūsų organizacijos abonementas jau prisijungęs šiame kompiuteryje" "Office"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Prisijungimo trikčių šalinimas naudojant "Office" šiuolaikinės autentifikavimas naudojant ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)