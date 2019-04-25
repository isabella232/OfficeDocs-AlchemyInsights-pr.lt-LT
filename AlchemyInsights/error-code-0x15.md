---
title: Klaidos kodas 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402747"
---
Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą. 
  
|**Registro raktas**|**Tipas**|**Vertė**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Daugiau informacijos ieškokite [Įjungti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Alma yra įjungta pagal nutylėjimą "Office 365 ProPlus" ir Office 2016. > nuotolinio darbalaukio tarnybų (RDS) anksčiau buvo pavadintas Terminal Services. 
  

