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
description: Jei aktyvindami "Office" nuotolinio darbalaukio tarnybų (RDS) diegimus gaunate klaidą, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316694"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Klaida aktyvinant 2013 Office. nuotolinio darbalaukio tarnybose

Jei aktyvindami "Office" nuotolinio darbalaukio tarnybų (RDS) diegimus gaunate klaidą, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.
  
|**Registro raktas**|**Tipas**|**Reikšmė**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daugiau informacijos žr. [2013 m. Office autentifikavimo įgalinimo Windows įrenginiuose.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Pastaba:** pagal numatytuosius nustatymus ADAL įjungiama 2016 m. "Microsoft 365" programos įmonėms Office. Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintos terminalo paslaugomis.
  