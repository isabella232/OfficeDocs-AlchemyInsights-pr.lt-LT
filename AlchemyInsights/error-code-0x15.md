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
<span data-ttu-id="2ea4e-103">Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="2ea4e-104">**Registro raktas**</span><span class="sxs-lookup"><span data-stu-id="2ea4e-104">**Registry key**</span></span>|<span data-ttu-id="2ea4e-105">įveskite</span><span class="sxs-lookup"><span data-stu-id="2ea4e-105">**Type**</span></span>|<span data-ttu-id="2ea4e-106">Reikšmė</span><span class="sxs-lookup"><span data-stu-id="2ea4e-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2ea4e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="2ea4e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="2ea4e-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="2ea4e-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="2ea4e-109">1</span><span class="sxs-lookup"><span data-stu-id="2ea4e-109">1</span></span>  <br/> |
   
<span data-ttu-id="2ea4e-110">Daugiau informacijos ieškokite [Įjungti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="2ea4e-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="2ea4e-p101">Alma yra įjungta pagal nutylėjimą "Office 365 ProPlus" ir Office 2016. > nuotolinio darbalaukio tarnybų (RDS) anksčiau buvo pavadintas Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

