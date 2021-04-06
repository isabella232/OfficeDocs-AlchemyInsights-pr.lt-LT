---
title: "\"Windows\" virtualiojo darbalaukio problemų šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595853"
---
# <a name="identify-windows-virtual-desktop-issues"></a>"Windows" virtualiojo darbalaukio problemų šalinimas

"Windows Virtual Desktop Diagnostics" naudoja tik vieną "PowerShell" "cmdlet", tačiau joje yra daug pasirinktinių parametrų, kurie padeda susiaurinti ir atskirti problemas. Norėdami pradėti: 

1. Atsisiųskite ir importuokite "Windows Virtual Desktop PowerShell" modulį. Daugiau informacijos žr. ["Windows Virtual Desktop Cmdlet", skirta "Windows PowerShell".](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Norėdami prisijungti prie savo paskyros, vykdykite šią "cmdlet":
    
    Pavyzdys: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**PASTABA:** Visose užklausose, kuriose naudojama "PowerShell", turi būti -UserName arba -ActivityID parametrai. Stebėjimo galimybes žr. [Žurnalo analizės naudojimas diagnostikos funkcijai](https://go.microsoft.com/fwlink/?linkid=2126847).

Norėdami filtruoti diagnostines veiklas pagal vartotoją, vykdykite šią "cmdlet":

Pavyzdys: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Yra filtrų, kuriuos galite naudoti problemoms diagnozuoti, sąrašas. Norėdami sužinoti daugiau apie problemų diagnozavimo klausimus, [žr. "Windows" virtualiojo darbalaukio](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)problemų šalinimas ir diagnostika.

Norėdami sužinoti daugiau apie įprastas klaidas, [žr. Bendrosios klaidos senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
