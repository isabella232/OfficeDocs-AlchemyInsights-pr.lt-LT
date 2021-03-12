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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708070"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinchronizavimo klaidos dėl pasikartojančių objektų

Galite gauti vieną iš šių klaidos žinučių, kai katalogų sinchronizavimas yra "Microsoft 365":

- Negalima atnaujinti šio objekto "Microsoft Online Services", nes toliau nurodyti atributai, susiję su šiuo objektu, turi reikšmes, kurios gali būti jau susietos su kitu objektu jūsų vietiniame kataloge.

- Sinchronizuotas objektas su tuo pačiu tarpinio serverio adresu jau yra jūsų "Microsoft Online Services" kataloge.

- Negalima naujinti šio objekto, nes toliau nurodyti atributai, susiję su šiuo objektu, turi reikšmes, kurios gali būti jau susietos su kitu objektu jūsų vietinio katalogo tarnybose: UserPrincipalName.

Norėdami nustatyti ir išspręsti šią problemą, atsisiųskite ir paleiskite " [IDFix DirSync" klaidų taisymo įrankį](https://github.com/Microsoft/idfix).

Daugiau informacijos ieškokite [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
