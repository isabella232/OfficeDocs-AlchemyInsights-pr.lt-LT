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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929096"
---
<span data-ttu-id="f0c8e-103">Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą.</span><span class="sxs-lookup"><span data-stu-id="f0c8e-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="f0c8e-104">**Registro raktas**</span><span class="sxs-lookup"><span data-stu-id="f0c8e-104">**Registry key**</span></span>|<span data-ttu-id="f0c8e-105">**Tipas**</span><span class="sxs-lookup"><span data-stu-id="f0c8e-105">**Type**</span></span>|<span data-ttu-id="f0c8e-106">**Reikšmė**</span><span class="sxs-lookup"><span data-stu-id="f0c8e-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f0c8e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f0c8e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f0c8e-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f0c8e-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f0c8e-109">1</span><span class="sxs-lookup"><span data-stu-id="f0c8e-109">1</span></span>  <br/> |
   
<span data-ttu-id="f0c8e-110">Daugiau informacijos ieškokite [Įjungti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f0c8e-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f0c8e-p101">Alma yra įjungta pagal nutylėjimą "Office 365 ProPlus" ir Office 2016. > nuotolinio darbalaukio tarnybų (RDS) anksčiau buvo pavadintas Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="f0c8e-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

