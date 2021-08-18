---
title: DKIM nustatymas naudojant pasirinktinius domenus
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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332315"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM nustatymas naudojant pasirinktinius domenus

Turite publikuoti du CNAME įrašus kiekvienam pasirinktiniam domenui DNS. Norėdami tai padaryti, naudokite šį formatą:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Pastaba:** **DomainGUID** yra tekstas į kairę **nuo .mail.protection.outlook.com** pasirinktinio domeno tinkintame MX įraše (pvz., contoso-com domeno **contoso.com**). **InitialDomain** yra domenas, kurį naudojote prisiregistravę naudoti Office 365 (pvz., **contoso.onmicrosoft.com**).

Daugiau informacijos apie DNS įrašus žr. [DNS įrašų kūrimas bet kuriame DNS išteklių nuomos teikėjo Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).