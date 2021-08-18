---
title: Išorinio automatinio el. pašto peradresavimo blokavimas arba atblokavimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315882"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokuoti arba atblokuoti amžinąjį automatinį el. pašto peradresavimą

Norėdami įjungti arba išjungti konkrečios pašto dėžutės el. pašto peradresavimą, žr. [El. pašto peradresavimo konfigūravimas](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Administratoriai gali valdyti išorinį organizacijos peradresavimą naudodami [siunčiamų pašto šiukšlių strategijas.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Siunčiamų pašto šiukšlių strategijas galite valdyti ""Microsoft 365" sargyba" portale <https://security.microsoft.com/antispam> "PowerShell" naudodami ["cmdlet Get-HostedOutboundSpamFilterPolicy"](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) "Exchange Online".

Jei gaunate šį klaidos **pranešimą: "550 5.7.520 Prieiga uždrausta,** Jūsų organizacija neleidžia išorinio peradresavimo" , įsitikinkite, kad strategija sukonfigūruota taip, kad įgalintumėte išorinius automatiškai peradresuojamus laiškus.

**Pastaba:** mes rekomendavome numatytąją **reikšmę**  Automatinis – sistema, valdoma pagal automatinio peradresavimo taisyklių parametrą numatytojoje siunčiamų pašto šiukšlių filtro politikoje (automatinis išorinis peradresavimas užblokuotas; vidinis automatinis peradresavimas vis tiek veikia). Turėtumėte sukurti pasirinktines siunčiamų pašto šiukšlių filtro strategijas ir naudoti reikšmę **Įjungta –** peradresavimas įgalintas tik vartotojams, kuriems reikia išorinio automatinio el. pašto peradresavimo. Daugiau informacijos žr. [Išorinio el. pašto peradresavimo konfigūravimas Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
