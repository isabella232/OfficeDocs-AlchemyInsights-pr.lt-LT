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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007690"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>ATNAUJINKITE DNS įrašus, kad jūsų svetainė būtų su dabartiniu išteklių nuomos teikėju

1. Puslapio "Microsoft 365" administravimo centras, eikite į puslapį Nustatyti domenus, o domenų sąraše pasirinkite domeną,  >  [](https://admin.microsoft.com/Adminportal#/Domains) kurį naudojate savo žiniatinklio svetainei.

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
