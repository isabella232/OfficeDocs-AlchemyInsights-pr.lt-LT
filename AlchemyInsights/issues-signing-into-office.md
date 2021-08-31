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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744654"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Prisijungimo prie ""Microsoft 365" programos

Pastaba: jei naudojate senesnę "Windows" versiją (pvz., "Windows 7" SP1, "Windows Server 2008 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) R2"), naudokite paprastą pataisą, kad įgalintumėte TLS 1.2 kaip numatytuosius parametrus. Daugiau informacijos žr. Naujinimas, kad [įgalintumėte TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Norėdami išspręsti prisijungimo problemas su Microsoft 365 programėlėmis, išbandykite šias parinktis paveiktame kompiuteryje:  

- Jei Windows, [žr. Rekomendacijos apie dažniausiai pasitaikančių prisijungimo problemų sprendimą](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Jei reikia "Mac", [žr. Negaliu prisijungti prie "Office 2016 for Mac" taikomosios programos](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Patarimas** „Windows“ kompiuteriuose galime diagnozuoti ir automatiškai už jus išspręsti kelias bendrąsias „Office“ prisijungimo problemas. Atsisiųskite ir paleiskite **[„Microsoft“ palaikymo ir atkūrimo pagalbinę priemonę](https://aka.ms/SaRA-OfficeSignInScenario)**, kad būtų galima naudoti mūsų automatinį įrankį.

**Pastaba:** Nerekomenduojama išjungti šiuolaikinio autentifikavimo (ADAL) arba žiniatinklio paskyros valdymo (WAM) prisijungimo arba **aktyvinimo problemų.** Jei klaidos įvyksta jungiantis prie "Microsoft 365" Office 2013", įsitikinkite, [kad](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) įgalinsite modernų "Office autentifikavimą.

Konkrečius trikčių šalinimo veiksmus žr.:

[Prisijungimo problemos atnaujinus į "Office 2016" komponavimo versiją 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Negalite prisijungti prie savo organizacijos paskyros, pvz., "Office 365", "Azure" arba "Intune"](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Kaip šalinti ne naršyklės programų, kurios negali prisijungti prie "Office 365", "Azure" arba "Intune", triktis](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Pakartotinai raginama įvesti kredencialus Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)