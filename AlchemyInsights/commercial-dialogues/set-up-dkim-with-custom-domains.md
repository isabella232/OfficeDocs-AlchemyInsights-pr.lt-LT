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
# <a name="set-up-dkim-with-custom-domains"></a>DKIM nustatymas su pasirinktiniais domenais

Kiekvienam pasirinktiniam domenui DNS turite publikuoti du CNAME įrašus. Norėdami tai padaryti, naudokite šį formatą:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **Domenasguid** yra pasirinktinio domeno PRITAIKYTAME MX įraše esantis tekstas į kairę nuo **. mail.Protection.Outlook.com** (pvz., "Contoso-com" domeno **contoso.com**). " **Initialdomain** " yra domenas, kurį naudojote, kai prisiregistravote naudoti "Office 365" (pvz., **contoso.onmicrosoft.com**).

Daugiau informacijos apie DNS įrašus ieškokite [DNS įrašų kūrimas "Office 365" DNS išteklių nuomos teikėjo](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)svetainėje.