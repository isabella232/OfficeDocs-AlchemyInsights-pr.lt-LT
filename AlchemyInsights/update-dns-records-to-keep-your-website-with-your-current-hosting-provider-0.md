---
title: Atnaujinkite DNS įrašus, kad jūsų svetainė būtų išsaugota su dabartiniu išteklių nuomos teikėju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665768"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atnaujinkite DNS įrašus, kad jūsų svetainė būtų išsaugota su dabartiniu išteklių nuomos teikėju

1. "Microsoft 365" administravimo centre eikite į puslapį **Sąrankos**  >  [domenai](https://portal.office.com/adminportal/home#/Domains) ir domenų sąraše pasirinkite domeną, kurį naudojate savo svetainei.

2. Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:

  - **DNS tipui** įveskite: **A (adresas)**

  - Pagrindinio **kompiuterio vardą arba pseudonimą**įveskite:**@**

  - **IP adresui**įveskite svetainės, kurioje šiuo metu nuomojama, statinį IP adresą (pvz., 172.16.140.1).

    Tai turi būti *statinis* IP adresas svetainėje, o ne *dinaminis* IP adresas. Pasitarkite su svetaine, kurioje nuomojama jūsų svetainė, kad įsitikintumėte, jog galite gauti statinį viešosios žiniatinklio svetainės IP adresą.

3. Pasirinkite **I¹saugoti**.

Be to, galite sukurti CNAME įrašą, kad padėtumėte klientams rasti jūsų svetainę.
  
1. Pasirinkite **+ Naujas pasirinktinis įrašas** ir įveskite:

  - **DNS tipui** įveskite: **CNAME (pseudonimas)**

  - Pagrindinio **kompiuterio vardą arba pseudonimą**įveskite: **www**

  - Jei **norite, kad nukreipia adresu**, įveskite visiškai apibrėžtą domeno vardą (FQDN) savo svetainei (pvz., contoso.com).

2. Pasirinkite **I¹saugoti**.
