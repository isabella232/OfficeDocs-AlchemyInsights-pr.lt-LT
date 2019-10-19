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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529027"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="e529a-102">OnChange įvykis nevyksta, jei laukas pakeičiamas programiškai</span><span class="sxs-lookup"><span data-stu-id="e529a-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="e529a-103">Įvykio *OnChange* nepasitaiko, jei laukas pakeičiamas programiškai naudojant *atributą.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodas.</span><span class="sxs-lookup"><span data-stu-id="e529a-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="e529a-104">Jei norite, kad įvykio apdorojimo programos, skirtos " *OnChange* ", būtų paleistas nustačius reikšmę, turite naudoti *atributą formcontext. data. Entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodas jūsų kodas.</span><span class="sxs-lookup"><span data-stu-id="e529a-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
