---
title: Dynamics 365 sudaro verslo taisyklės - verslo taisyklės ne šaudyti formos
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748203"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange atveju kyla ne programiškai pakeitus lauko

*OnChange* atveju neiškyla jei lauką pasikeičia programiškai naudojant į *atributo.* [Nustatyti_reikšmę](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodas. Jei norite, kad įvykio apdorojimo programos, *OnChange* atveju vykdyti po to, kai nustatote vertę, turite naudoti su *formContext.data.entity atributo.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodas savo kodą.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
