---
title: 726 El. pašto peradresavimo blokavimas
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059640"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>El. pašto peradresavimo blokavimas arba atblokavimas

Norėdami įjungti arba išjungti konkrečios pašto dėžutės el. pašto peradresavimą, žr. [El. pašto peradresavimo konfigūravimas](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Nuomotojo lygiu išorinio peradresavimo valdymas atliekamas naudojant siunčiamų pašto šiukšlių strategiją. Siunčiamų pašto šiukšlių filtro strategiją galite patikrinti [](https://protection.office.com/antispam) čia arba naudodami [komandą Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Jei gaunate šią klaidą: **"550 5.7.520 Prieiga uždrausta,** Jūsų organizacija neleidžia išorinio peradresavimo", įsitikinkite, kad strategija sukonfigūruota taip, kad įgalintumėte išorinį automatinį persiuntimą.

**Pastaba:** Rekomenduojama išjungti išorinį automatinį paleidimą numatytoje siunčiamų pašto šiukšlių filtro politikoje ir įgalinti ją tik vartotojams, kuriems reikia išorinio peradresavimo, sukuriant pasirinktinę strategiją tiems vartotojams. Daugiau informacijos galite perskaityti [lauke Išorinio el. pašto peradresavimo konfigūravimas Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)