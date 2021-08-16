---
title: Klaidos kodo 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jei 2013 m. "Office tarnybų (RDS) diegimų aktyvinimo metu gaunate klaidą, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100770"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Klaida aktyvinant 2013 Office. nuotolinio darbalaukio tarnybose

Jei 2013 m. "Office tarnybų (RDS) diegimų aktyvinimo metu gaunate klaidą, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.
  
|**Registro raktas**|**Tipas**|**Reikšmė**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daugiau informacijos žr. [2013 m. Office autentifikavimo įgalinimo Windows įrenginiuose.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  Pagal numatytuosius nustatymus ADAL įjungiama "Microsoft 365" programos įmonėms 2016 Office. Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintos terminalo paslaugomis.
  