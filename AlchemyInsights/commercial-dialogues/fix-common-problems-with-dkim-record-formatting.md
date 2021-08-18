---
title: Dažniausiai pasitaikančių DKIM įrašų formatavimo problemų sprendimas
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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323998"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Dažniausiai pasitaikančių DKIM įrašų formatavimo problemų sprendimas

Dauguma DKIM set-up problemų yra susijusios su netinkamais DNS įrašais.

Norėdami išspręsti DKIM rinkinio problemas, patikrinkite, ar tinkamai suformatuotas DKIM CNAME įrašas **(ne** TXT įrašas). Daugiau informacijos žr. Ką reikia daryti norint rankiniu būdu nustatyti [DKIM "Office 365".](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Jei reikia pagalbos dėl DNS įrašų apskritai, žr. [DNS įrašų kūrimas bet kuriame DNS išteklių](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)nuomos teikėjo Office 365 .

**Pastaba:** sukūrę arba atnaujinę DKIM DNS įrašus savo domeno DNS išteklių nuomos paslaugoje, turėsite palaukti, kol bus platinami DNS įrašai.
