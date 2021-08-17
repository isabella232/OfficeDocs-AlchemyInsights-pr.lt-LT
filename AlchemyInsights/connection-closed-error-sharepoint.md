---
title: Pagrindinio ryšio klaida buvo uždaryta SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883327"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Klaida "Pagrindinis ryšys buvo uždarytas" SharePoint

Jei gaunate klaidos pranešimą "Pagrindinis ryšys buvo uždarytas" SharePoint jis gali būti susijęs su TLS 1.0/1.1 nutraukimu. Daugiau informacijos žr. šiuose straipsniuose:

- [Pasirengimas TLS 1.2 Office 365 ir Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Autentifikavimo klaidos įvyksta, jei klientas nepalaiko TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jei vartotojai yra 7 Windows, įsitikinkite, kad [jie "TLS Cipher Suites" Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)