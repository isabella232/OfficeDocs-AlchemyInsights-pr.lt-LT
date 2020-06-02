---
title: Klaidos kodas 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jei gaunate klaidos pranešimą aktyvinant "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimuose, apsvarstykite galimybę įgalinti Alma redaguodami registrą.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506854"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="964f4-103">Aktyvinimo "Office 2013" nuotolinio darbalaukio tarnybose klaida</span><span class="sxs-lookup"><span data-stu-id="964f4-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="964f4-104">Jei gaunate klaidos pranešimą aktyvinant "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimuose, apsvarstykite galimybę įgalinti Alma redaguodami registrą.</span><span class="sxs-lookup"><span data-stu-id="964f4-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="964f4-105">**Registro raktas**</span><span class="sxs-lookup"><span data-stu-id="964f4-105">**Registry key**</span></span>|<span data-ttu-id="964f4-106">**Tipas**</span><span class="sxs-lookup"><span data-stu-id="964f4-106">**Type**</span></span>|<span data-ttu-id="964f4-107">**Vertė**</span><span class="sxs-lookup"><span data-stu-id="964f4-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="964f4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="964f4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="964f4-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="964f4-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="964f4-110">1</span><span class="sxs-lookup"><span data-stu-id="964f4-110">1</span></span>  <br/> |

<span data-ttu-id="964f4-111">Daugiau informacijos [ieškokite Modern Authentication for Office 2013 " Windows " įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="964f4-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="964f4-112">Pagal numatytuosius nustatymus ADAL įgalintas "Microsoft 365" programose, skirtose įmonėms ir "Office 2016".</span><span class="sxs-lookup"><span data-stu-id="964f4-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="964f4-113">Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintas terminalų tarnybos.</span><span class="sxs-lookup"><span data-stu-id="964f4-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  