---
title: "\"Dynamics 365 Forms Business\" taisyklės – \"Business Rule Not Firing for a Form\""
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947307"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>"OnChange" įvykis neįvyksta, jei laukas pakeičiamas programiškai

Įvykis *"OnChange"* neįvyksta, jei laukas programiškai pakeičiamas naudojant *atributą.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodas. Jei norite, kad įvykio *OnChange* įvykių apdorojimo programos būtų paleisto po to, kai nustatote reikšmę, turite naudoti *formContext.data.entity atributo* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodą savo kode.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
