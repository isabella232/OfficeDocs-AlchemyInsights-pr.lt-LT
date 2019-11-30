---
title: Duomenų vieta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627854"
---
# <a name="data-location"></a>Duomenų vieta

Galite peržiūrėti savo "Office 365" nuomotojo vietą administravimo centre arba prisijungti prie "Exchange Online" per "PowerShell".


**Administravimo centras:**
1. Prisijunkite prie [administravimo centro](https://admin.microsoft.com/Adminportal/Home).
2. Pasirinkite **Parametrai** > **organizacijos profilis**.
3. Dalyje **duomenų vieta**pasirinkite **Peržiūrėti išsamią informaciją**.


**Powershell:**
1. Prisijungti prie Exchange Online naudojant "Windows PowerShell".
2. Vykdyti [gauti-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet Rodyti savo nuomotojo ypatybes sąrašą. 
3. Peržiūrėkite ypatybę OrganizationId.

Jei turite EXO ir SPO duomenų vietą, galite nustatyti duomenų vietą kitoms paslaugoms, kurias galite naudoti iš [ten, kur yra jūsų duomenys](https://products.office.com/where-is-your-data-located).