---
title: 902 (Sinchronizavimo klaidos dėl pasikartojančių objektų)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998802"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinchronizavimo klaidos dėl pasikartojančių objektų

Kai katalogų sinchronizavimas baigiamas naudojant "Microsoft 365", galite gauti vieną iš šių Microsoft 365:

- Nepavyko atnaujinti šio objekto "Microsoft Online Services", nes toliau nurodyti atributai, susiję su šiuo objektu, turi reikšmes, kurios gali būti susietos su kitu objektu jūsų vietiniame kataloge.

- Sinchronizuotas objektas su tuo pačiu tarpinio serverio adresu jau yra jūsų "Microsoft Online Services" kataloge.

- Nepavyko atnaujinti šio objekto, nes šie su šiuo objektu susieti atributai turi reikšmes, kurios jau gali būti susietos su kitu objektu vietinės katalogų tarnybose: UserPrincipalName.

Norėdami nustatyti ir išspręsti šią problemą, atsisiųskite ir paleiskite ["IdFix DirSync" klaidų atkūrimo įrankį](https://github.com/Microsoft/idfix).

Daugiau informacijos žr. [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
