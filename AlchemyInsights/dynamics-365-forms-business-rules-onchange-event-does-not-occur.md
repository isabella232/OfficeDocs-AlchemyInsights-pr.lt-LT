---
title: Dynamics 365 formos verslo taisyklės-verslo taisyklės nešaudo formos
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769347"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange įvykis nevyksta, jei laukas pakeičiamas programiškai

Įvykio *OnChange* nepasitaiko, jei laukas pakeičiamas programiškai naudojant *atributą.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodas. Jei norite, kad įvykio apdorojimo programos įvykio *OnChange* paleisti po to, kai nustatote reikšmę turite naudoti *formcontext. data. Entity atributas* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) kodą.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
