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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Aktyvinimo "Office 2013" nuotolinio darbalaukio tarnybose klaida

Jei gaunate klaidos pranešimą aktyvinant "Office 2013" nuotolinio darbalaukio tarnybų (RDS) diegimuose, apsvarstykite galimybę įgalinti Alma redaguodami registrą.
  
|**Registro raktas**|**Tipas**|**Vertė**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Daugiau informacijos [ieškokite Modern Authentication for Office 2013 " Windows " įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Pagal numatytuosius nustatymus ADAL įgalintas "Microsoft 365" programose, skirtose įmonėms ir "Office 2016". Nuotolinio darbalaukio tarnybos (RDS) anksčiau buvo pavadintas terminalų tarnybos.
  