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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="c064e-103">Klaida aktyvinant "Office 2013" nuotolinio darbalaukio tarnybose</span><span class="sxs-lookup"><span data-stu-id="c064e-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="c064e-104">Jei gaunate klaidą aktyvindami "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimus, apsvarstykite galimybę įgalinti ADAL redaguodami registrą.</span><span class="sxs-lookup"><span data-stu-id="c064e-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="c064e-105">**Registro raktas**</span><span class="sxs-lookup"><span data-stu-id="c064e-105">**Registry key**</span></span>|<span data-ttu-id="c064e-106">**Įveskite**</span><span class="sxs-lookup"><span data-stu-id="c064e-106">**Type**</span></span>|<span data-ttu-id="c064e-107">**Reikšmę**</span><span class="sxs-lookup"><span data-stu-id="c064e-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c064e-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="c064e-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="c064e-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="c064e-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="c064e-110">1</span><span class="sxs-lookup"><span data-stu-id="c064e-110">1</span></span>  <br/> |

<span data-ttu-id="c064e-111">Daugiau informacijos rasite " [Office 2013" šiuolaikinės autentifikavimo įgalinimas "Windows" įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c064e-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="c064e-112">"ADAL" įgalintas pagal numatytuosius "Microsoft" 365 "Enterprise" ir "Office 2016" programose.</span><span class="sxs-lookup"><span data-stu-id="c064e-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="c064e-113">Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintos terminalų tarnybomis.</span><span class="sxs-lookup"><span data-stu-id="c064e-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  