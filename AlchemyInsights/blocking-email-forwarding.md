---
title: 726 blokavimo el. pašto peradresavimas
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478345"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Pašto peradresavimo blokavimas arba atblokavimas

Norėdami įjungti arba išjungti konkrečios pašto dėžutės pašto peradresavimą, skaitykite [pašto peradresavimo konfigūravimas](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Nuomotojo lygmenyje išorinio peradresavimo valdymas atliekamas naudojant siuntimo pašto šiukšlių strategiją. Galite patikrinti siuntimo pašto šiukšlių filtravimo strategiją iš saugos ir atitikties centro [čia](https://protection.office.com/antispam) arba naudodami [komandą Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Jei gaunate šį klaidos pranešimą: **"550 5.7.520" prieiga uždrausta, jūsų organizacija neleidžia naudoti išorinio peradresavimo "**, įsitikinkite, kad strategija sukonfigūruota įgalinti išorinį automatinį persiuntimą.

**Pastaba:** Rekomenduojama palikti išorinį automatinį persiuntimą jūsų numatytoje siuntimo pašto šiukšlių filtro strategijoje ir įgalinti ją tik vartotojams, kuriems reikia išorinio persiuntimo sukuriant pasirinktinę strategiją tiems vartotojams. Galite paskaityti daugiau [konfigūravus išorinį pašto persiuntimą "Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)".