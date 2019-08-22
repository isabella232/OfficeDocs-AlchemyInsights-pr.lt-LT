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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529027"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="3ab3f-102">OnChange atveju kyla ne programiškai pakeitus lauko</span><span class="sxs-lookup"><span data-stu-id="3ab3f-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="3ab3f-103">*OnChange* atveju neiškyla jei lauką pasikeičia programiškai naudojant į *atributo.* [Nustatyti_reikšmę](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodas.</span><span class="sxs-lookup"><span data-stu-id="3ab3f-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="3ab3f-104">Jei norite, kad įvykio apdorojimo programos, *OnChange* atveju vykdyti po to, kai nustatote vertę, turite naudoti su *formContext.data.entity atributo.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodas savo kodą.</span><span class="sxs-lookup"><span data-stu-id="3ab3f-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
