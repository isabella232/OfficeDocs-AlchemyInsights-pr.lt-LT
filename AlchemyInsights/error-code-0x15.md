---
title: Klaidos kodas 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499390"
---
Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą. 
  
|**Registro raktas**|įveskite|Reikšmė|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Daugiau informacijos ieškokite [Įjungti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Alma yra įjungta pagal nutylėjimą "Office 365 ProPlus" ir Office 2016. > nuotolinio darbalaukio tarnybų (RDS) anksčiau buvo pavadintas Terminal Services. 
  

