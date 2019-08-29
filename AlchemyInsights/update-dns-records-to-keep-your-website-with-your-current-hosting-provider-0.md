---
title: Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665768"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas

1. "Microsoft" 365 administravimo centro, eikite į **nustatymas** > [domenai](https://portal.office.com/adminportal/home#/Domains) puslapio ir domenų sąrašą, pasirinkite domeno, jūs naudojate savo svetainę.

2. Pasirinkite **+ naują vartotojo įrašą** ir įveskite šiuos veiksmus:

  - **DNS** tipo įveskite: **(adresas)**

  - **Pagrindinio kompiuterio vardą arba pseudonimą**, įveskite:**@**

  - **IP adresą**, įveskite statinį IP adresą į savo svetainę, kur ji šiuo metu yra Patalpinta (pavyzdžiui, 172.16.140.1).

    Tai turi būti svetainės, ne *dinaminis* IP adresas yra *statinis* IP adresas. Teiraukitės svetainę kur jūsų svetainė hosted įsitikinkite, kad jums yra Statinis IP adresas, jūsų viešąją žiniatinklio svetainę.

3. Pasirinkite **įrašyti**.

Be to, sukuriate CNAME įrašą, padėti klientams surasti jūsų svetainę.
  
1. Pasirinkite **+ naują vartotojo įrašą** ir įveskite šiuos veiksmus:

  - **DNS** tipo įveskite: **CNAME (pseudonimas)**

  - **Pagrindinio kompiuterio vardą arba pseudonimą**, įveskite: **www**

  - **Atkreipia dėmesį į adresą**, įrašykite visiškai apibrėžtą domeno vardą (FQDN) į savo svetainę (pvz.,.: contoso.com).

2. Pasirinkite **įrašyti**.
