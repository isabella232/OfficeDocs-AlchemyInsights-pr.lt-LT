---
title: Klaidos kodas 0x15
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
description: Jei gaunate klaidą aktyvindami "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimus, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709195"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Klaida aktyvinant "Office 2013" nuotolinio darbalaukio tarnybose

Jei gaunate klaidą aktyvindami "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimus, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.
  
|**Registro raktas**|**Įveskite**|**Reikšmę**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Daugiau informacijos rasite " [Office 2013" šiuolaikinės autentifikavimo įgalinimas "Windows" įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  "ADAL" įgalintas pagal numatytuosius "Microsoft" 365 "Enterprise" ir "Office 2016" programose. Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintos terminalų tarnybomis.
  