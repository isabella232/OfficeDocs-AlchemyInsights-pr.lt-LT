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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="5f2db-102">OnChange atveju kyla ne programiškai pakeitus lauko</span><span class="sxs-lookup"><span data-stu-id="5f2db-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="5f2db-103">*OnChange* atveju neiškyla jei lauką pasikeičia programiškai naudojant į *atributo.* [Nustatyti_reikšmę](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodas.</span><span class="sxs-lookup"><span data-stu-id="5f2db-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="5f2db-104">Jei norite, kad įvykio apdorojimo programos, *OnChange* atveju vykdyti po to, kai nustatote vertę, turite naudoti su *formContext.data.entity atributo.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodas savo kodą.</span><span class="sxs-lookup"><span data-stu-id="5f2db-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
