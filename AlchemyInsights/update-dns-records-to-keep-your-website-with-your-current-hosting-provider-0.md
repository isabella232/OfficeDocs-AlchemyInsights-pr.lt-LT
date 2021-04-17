---
title: ATNAUJINKITE DNS įrašus, kad jūsų svetainė būtų su dabartiniu išteklių nuomos teikėju
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827534"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>ATNAUJINKITE DNS įrašus, kad jūsų svetainė būtų su dabartiniu išteklių nuomos teikėju

1. "Microsoft 365" administravimo centre eikite į puslapį Domenų sąranka, o domenų sąraše pasirinkite domeną,  >  [](https://admin.microsoft.com/Adminportal#/Domains) kurį naudojate savo žiniatinklio svetainei.

2. Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:

  - **Jei norite įvesti DNS** tipą: A **(Adresas)**

  - Jei **tai pagrindinio kompiuterio vardas arba pseudonimas,** įveskite: **@**

  - **Jei norite naudoti IP** adresą, įveskite statinį svetainės, kurioje jis šiuo metu nuomojamas, IP adresą (pvz., 172.16.140.1).

    Tai turi būti  *statinis svetainės*  IP adresas, o ne  *dinaminis*  IP adresas. Patikrinkite svetainę, kurioje laikoma jūsų svetainė, kad įsitikintumėte, jog galite gauti statinį viešosios žiniatinklio svetainės IP adresą.

3. Pasirinkite **Įrašyti**.

Be to, galite sukurti CNAME įrašą, kad klientai galėtų rasti jūsų svetainę.
  
1. Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:

  - **Jei norite įvesti DNS** tipą: **CNAME (pseudonimas)**

  - Jei **reikia pagrindinio kompiuterio vardo arba pseudonimo,** įveskite: **www**

  - Dalyje **Adreso taškai** įveskite visiškai apibrėžtą savo svetainės domeno vardą (FQDN) (pvz., contoso.com).

2. Pasirinkite **Įrašyti**.
