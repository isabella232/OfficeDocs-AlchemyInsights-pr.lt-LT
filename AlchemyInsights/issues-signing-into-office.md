---
title: Problemos prisijungiant prie "Office" programos
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938278"
---
# <a name="issues-signing-in-to-office-apps"></a>Problemos prisijungiant prie "Office" programos

Norėdami išspręsti prisijungimo problemas su "Office" programos, pabandykite atlikti šiuos veiksmus:

- Pašalinti visas darbo sąskaitas, išskyrus paveiktą paskyrą, naudodami "Windows" parametrus > **prieigos darbe ar mokykloje**.
- [Aišku Office kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvas.<br/>
    **Pastaba:** 16,0 pasikeitė registro maršrutai Office 2016. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Atidaryti Office programą, pasirinkite **failą** > **į** > **Atsijungti**. Tada prisijunkite naudodami vartotojo abonementą, turintis galiojančią licenciją. Išsamios informacijos, peržiūrėkite [sąskaitas savo pareigas](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Skirta "Mac", žr. [negaliu prisijungti prie Office 2016 Mac App](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Jei klaidos atsiranda, o jungiantis prie Office 2013 naudojant "Office 365", leidžia šiuolaikinės autentifikavimas Office kliento.

Daugiau informacijos žr.
- [Jūs negalite prisijungti prie "Office 365", Azure arba Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Ryšį klausimai programoje prisijungdami po atnaujinimo į Office 2016, kurti 16.0.7967 "Windows 10"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Deja, kitą sąskaitą iš jūsų organizacija jau pasirašė šiame kompiuteryje" biure](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Spręsti prisijungimo problemas su Office šiuolaikinės autentifikavimas naudojant ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)