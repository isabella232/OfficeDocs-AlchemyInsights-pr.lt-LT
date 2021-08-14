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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930069"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Dažniausiai pasitaikančių DKIM įrašų formatavimo problemų sprendimas

Dauguma DKIM set-up problemų yra susijusios su netinkamais DNS įrašais.

Norėdami išspręsti DKIM rinkinio problemas, patikrinkite, ar tinkamai suformatuotas DKIM CNAME įrašas **(ne** TXT įrašas). Daugiau informacijos žr. Ką reikia daryti norint rankiniu būdu nustatyti [DKIM "Office 365".](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Jei reikia pagalbos dėl DNS įrašų apskritai, žr. DNS įrašų [kūrimas bet kuriame DNS išteklių](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)nuomos teikėjo Office 365 .

> [!NOTE]
> Sukūrę arba atnaujinę DKIM DNS įrašus savo domeno DNS išteklių nuomos paslaugoje, turėsite palaukti, kol bus platinami DNS įrašai.
