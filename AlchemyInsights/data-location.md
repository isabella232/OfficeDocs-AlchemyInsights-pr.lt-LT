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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655290"
---
# <a name="data-location"></a>Duomenų vieta

Galite peržiūrėti savo nuomotojo vietą administravimo centre arba prisijungę prie "Exchange Online" per "PowerShell".


**Administravimo centras:**
1. Prisijunkite prie [administravimo centro](https://admin.microsoft.com/Adminportal/Home).
2. Pasirinkite **Parametrai** > **Organizacijos profilis**.
3. Dalyje **Duomenų vieta**pasirinkite **Peržiūrėti išsamią informaciją**.


**Powershell:**
1. Prisijunkite prie "Exchange Online" naudodami "Windows PowerShell".
2. Vykdykite [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet, kad būtų rodomas nuomotojo ypatybių sąrašas. 
3. Pažvelkite į OrganizationId ypatybę.

Jei turite EXO ir SPO duomenų vietą, galite nustatyti kitų paslaugų, kurias galite [naudoti, duomenų](https://products.office.com/where-is-your-data-located)vietą iš Kur yra jūsų duomenys .