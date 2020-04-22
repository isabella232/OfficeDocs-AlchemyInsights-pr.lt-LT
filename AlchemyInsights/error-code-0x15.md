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
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703146"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="d7dfa-103">Aktyvinimo "Office 2013" nuotolinio darbalaukio tarnybose klaida</span><span class="sxs-lookup"><span data-stu-id="d7dfa-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="d7dfa-104">Jei gaunate klaidos pranešimą aktyvinant "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimuose, apsvarstykite galimybę įgalinti Alma redaguodami registrą.</span><span class="sxs-lookup"><span data-stu-id="d7dfa-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="d7dfa-105">**Registro raktas**</span><span class="sxs-lookup"><span data-stu-id="d7dfa-105">**Registry key**</span></span>|<span data-ttu-id="d7dfa-106">**Tipas**</span><span class="sxs-lookup"><span data-stu-id="d7dfa-106">**Type**</span></span>|<span data-ttu-id="d7dfa-107">**Vertė**</span><span class="sxs-lookup"><span data-stu-id="d7dfa-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d7dfa-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="d7dfa-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="d7dfa-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="d7dfa-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="d7dfa-110">1</span><span class="sxs-lookup"><span data-stu-id="d7dfa-110">1</span></span>  <br/> |

<span data-ttu-id="d7dfa-111">Daugiau informacijos [ieškokite Modern Authentication for Office 2013 " Windows " įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d7dfa-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d7dfa-112">Pagal numatytuosius nustatymus ADAL įgalintas "Microsoft 365" programose, skirtose įmonėms ir "Office 2016".</span><span class="sxs-lookup"><span data-stu-id="d7dfa-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="d7dfa-113">Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintas terminalų tarnybos.</span><span class="sxs-lookup"><span data-stu-id="d7dfa-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  