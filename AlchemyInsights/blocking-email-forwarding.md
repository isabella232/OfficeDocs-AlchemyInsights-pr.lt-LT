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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219863"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Pašto peradresavimo blokavimas arba atblokavimas

Norėdami įjungti arba išjungti konkrečios pašto dėžutės pašto peradresavimą, skaitykite [pašto peradresavimo konfigūravimas](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Nuomotojo lygiu išorinio peradresavimo valdymas atliekamas naudojant siuntimo pašto šiukšlių strategiją. Jei jis nustatytas kaip išjungtas arba automatinis, gali būti blokuojamų laiškų peradresavimas su klaida "550 5.7.520" prieiga uždrausta, jūsų organizacija neleidžia naudoti išorinio peradresavimo ". Vėliau, jei buvo nustatyta, kad peradresavimas yra užblokuotas, tai yra klaida, kurią matys vartotojai.

Jei peradresavimas užblokuotas, įsitikinkite, kad strategija sukonfigūruota įgalinti išorinius Autoforward. Galite patikrinti siuntimo pašto šiukšlių filtravimo strategiją iš saugos ir atitikties centro arba paleisdami komandą gauti HostedOutboundSpamFilterPolicy | FL pavadinimas, AutoForwardingMode. Jei norite nustatyti automatinį persiuntimą, ta pati komanda parodys jums strategijos būseną dabar.

Pastaba: rekomenduojama palikti išorinį automatinį persiuntimą jūsų numatytoje siuntimo pašto šiukšlių filtro strategijoje ir įgalinti ją tik vartotojams, kuriems reikia išorinio persiuntimo sukuriant pasirinktinę strategiją tiems vartotojams. Galite paskaityti daugiau [konfigūravus išorinį pašto persiuntimą "Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)".