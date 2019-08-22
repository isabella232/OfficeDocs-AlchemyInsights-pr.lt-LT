---
title: Klaidos kodas 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527026"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="4cfd2-103">Dėl nuotolinio darbalaukio tarnybos Office 2013 aktyvinimo klaida</span><span class="sxs-lookup"><span data-stu-id="4cfd2-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="4cfd2-104">Jei gaunate Klaida aktyvinant Office 2013 nuotolinio darbalaukio tarnybų (RDS) dislokavimo, patariame įjungti Alma redaguodami registrą.</span><span class="sxs-lookup"><span data-stu-id="4cfd2-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="4cfd2-105">**Registro raktas**</span><span class="sxs-lookup"><span data-stu-id="4cfd2-105">**Registry key**</span></span>|<span data-ttu-id="4cfd2-106">**Tipas**</span><span class="sxs-lookup"><span data-stu-id="4cfd2-106">**Type**</span></span>|<span data-ttu-id="4cfd2-107">**Vertė**</span><span class="sxs-lookup"><span data-stu-id="4cfd2-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4cfd2-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4cfd2-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4cfd2-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4cfd2-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4cfd2-110">1</span><span class="sxs-lookup"><span data-stu-id="4cfd2-110">1</span></span>  <br/> |

<span data-ttu-id="4cfd2-111">Daugiau informacijos ieškokite [Įjungti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4cfd2-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4cfd2-112">Alma yra įjungta pagal nutylėjimą "Office 365 ProPlus" ir Office 2016.</span><span class="sxs-lookup"><span data-stu-id="4cfd2-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="4cfd2-113">Nuotolinio darbalaukio tarnybų (RDS) anksčiau buvo pavadintas Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="4cfd2-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  