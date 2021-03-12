---
title: Bendrųjų problemų sprendimas naudojant DKIM įrašo formatavimą
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750763"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Bendrųjų problemų sprendimas naudojant DKIM įrašo formatavimą

Daugelis DKIM nustatymo problemų yra susijusios su klaidingais DNS įrašais.

Norėdami sutvarkyti DKIM nustatymo problemas, patikrinkite, ar teisingai suformatuotas DKIM CNAME įrašas (**ne** txt įrašas). Daugiau informacijos ieškokite [ką reikia daryti norint rankiniu būdu nustatyti DKIM "Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)".

Jei reikia pagalbos dėl DNS įrašų, ieškokite [DNS įrašų kūrimas bet kuriame DNS išteklių nuomos teikėjo, skirto "Office 365"](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Kai savo domeno DNS išteklių nuomos tarnyboje sukuriate arba naujinate savo DKIM DNS įrašus, turėsite palaukti, kol DNS įrašus išplatins.
