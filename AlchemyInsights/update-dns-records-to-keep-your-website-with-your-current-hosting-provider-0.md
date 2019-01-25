---
title: Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29480552"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Atnaujinti DNS įrašus laikyti savo svetainę su jūsų prieglobos paslaugų teikėjas

1. Puslapyje [domenai](https://portal.office.com/adminportal/home#/Domains) domenų, sąraše pažymėkite domeno naudojate savo svetainę, ir tada pasirinkite **DNS parametrus** valdymo srityje. 
    
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
    

