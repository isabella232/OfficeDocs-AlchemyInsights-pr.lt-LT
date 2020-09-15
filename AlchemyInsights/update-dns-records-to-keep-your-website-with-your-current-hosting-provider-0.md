---
title: Atnaujinkite DNS įrašus ir atnaujinkite savo svetainę su dabartiniu išteklių nuomos teikėju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699527"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atnaujinkite DNS įrašus ir atnaujinkite savo svetainę su dabartiniu išteklių nuomos teikėju

1. "Microsoft 365" administravimo centre eikite į puslapį **sąrankos**  >  [domenai](https://portal.office.com/adminportal/home#/Domains) ir domenų sąraše pasirinkite domeną, kurį naudojate savo žiniatinklio svetainei.

2. Pasirinkite **+ naujas tinkintas įrašas** ir įrašykite šiuos dalykus:

  - **DNS tipas** įveskite: **a (adresas)**

  - Jei esate **pagrindinio kompiuterio vardas arba pseudonimas**, įveskite: **@**

  - Jei naudojate **IP adresą**, įveskite savo žiniatinklio svetainės, kurioje yra šiuo metu Patalpinta, STATINĮ IP adresą (pvz.,: 172.16.140.1).

    Tai turi būti  *statinis*  IP adresas žiniatinklio svetainei, o ne  *dinaminis*  IP adresas. Patikrinkite svetainę, kurioje yra jūsų žiniatinklio svetainė, kad įsitikintumėte, jog galite gauti viešosios žiniatinklio svetainės statinį IP adresą.

3. Pasirinkite **įrašyti**.

Be to, galite sukurti CNAME įrašą, padėsiantį klientams rasti jūsų svetainę.
  
1. Pasirinkite **+ naujas tinkintas įrašas** ir įrašykite šiuos dalykus:

  - **DNS tipas** įveskite: **CNAME (pseudonimas)**

  - Jei esate **pagrindinio kompiuterio vardas arba pseudonimas**, įveskite: **www**

  - Jei **norite, kad būtų rodomas adresas**, įveskite savo žiniatinklio svetainės visiškai apibrėžtą domeno vardą (FQDN) (pvz., contoso.com).

2. Pasirinkite **įrašyti**.
