---
title: DKIM nustatymas su pasirinktiniais domenais
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747643"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="13811-102">DKIM nustatymas su pasirinktiniais domenais</span><span class="sxs-lookup"><span data-stu-id="13811-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="13811-103">Kiekvienam pasirinktiniam domenui DNS turite publikuoti du CNAME įrašus.</span><span class="sxs-lookup"><span data-stu-id="13811-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="13811-104">Norėdami tai padaryti, naudokite šį formatą:</span><span class="sxs-lookup"><span data-stu-id="13811-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="13811-105">**Domenasguid** yra pasirinktinio domeno PRITAIKYTAME MX įraše esantis tekstas į kairę nuo **. mail.Protection.Outlook.com** (pvz., "Contoso-com" domeno **contoso.com**).</span><span class="sxs-lookup"><span data-stu-id="13811-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="13811-106">" **Initialdomain** " yra domenas, kurį naudojote, kai prisiregistravote naudoti "Office 365" (pvz., **contoso.onmicrosoft.com**).</span><span class="sxs-lookup"><span data-stu-id="13811-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="13811-107">Daugiau informacijos apie DNS įrašus ieškokite [DNS įrašų kūrimas "Office 365" DNS išteklių nuomos teikėjo](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)svetainėje.</span><span class="sxs-lookup"><span data-stu-id="13811-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>